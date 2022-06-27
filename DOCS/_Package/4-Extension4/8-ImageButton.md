---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ImageButton Class
nav_order: 8
permalink: /package/extension4/imagebutton

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ImageButton.PNG" target="_blank">
<img src="/img/Package/Ext4-ImageButton.PNG" alt="login image"></a>

A class that displays an image button. Images and titles can be displayed on the surface of the button.

**Screen Display Example**

ButtonStyle = $STD
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_imagebutton.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

ButtonStyle = $SURFACE
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_imagebutton.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

ButtonStyle = $ICON
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_imagebutton.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

**Printer output by Doc class**<br>
It prints the same as the screen, but it does not reflect the button style. It is always printed without being pressed.

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/button/properties/value">Value</a>. ValueType can be String,Number,Fixed, Date and UString.<br><small><span style="color:green">UString has been added since Ver.4.2.0</span></small><br>

### Relationship between image and text display position <br>
The relationship between the set image and the characters specified in the  <a href="/package/standard/button/properties/title">Title</a> property is as follows by specifying the <a href="/package/standard/imagebutton/properties/vertplacement">VertPlacement</a> and <a href="/package/standard/imagebutton/properties/horzplacement">HorzPlacement</a> properties.

<a href="/img/Package/Ext4-ImageButton2.PNG" target="_blank">
<img src="/img/Package/Ext4-ImageButton2.PNG" alt="login image"></a>


Vertical and horizontal alignment with the <a href="/package/standard/imagebutton/properties/verticalalign">VerticalAlign</a> and <a href="/package/standard/imagebutton/properties/horizontalalign">HorizontalAlign</a> properties is performed while maintaining the above positional relationship.

If the <a href="/package/standard/imagebutton/properties/buttonstyle">ButtonStyle</a> property is $ICON and the VertPlacement and HorzPlacement properties are both $ CENTERED, no text is displayed inside the image, but text is displayed below the image. (VertPlacement property is the same display position as $ABOVETEXT)

The initial value of the margin (<a href="/package/standard/imagebutton/properties/spacing">Spacing</a> property) around the button is set to 5. Set the Spacing property to 0 if you want to have no margins.

**Limitations when visual style is enabled**<br>
◆ Specifying the visual style is invalid.


**Precautions when scaling**<br>
  ◆ The image displayed internally is also subject to scaling.





















