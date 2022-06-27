---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ImageLabel Class
nav_order: 9
permalink: /package/extension4/imagelabel

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ImageLabel.PNG" target="_blank">
<img src="/img/Package/Ext4-ImageLabel.PNG" alt="login image"></a>

A class that displays image labels. Images and text can be displayed on the surface of the label.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_imagelabel.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Printer output by Doc class**<br>
It will be printed in the same way as the screen.

The ruled line is a solid line, but it is printed according to the style only when the BorderStyle property is set to $DASH or $DOT.

Even if the UString type is specified for the data type, all characters are converted to multibyte when printing, so Unicode-specific characters are printed as "?".

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/label/properties/value">Value</a>. ValueType can be String,Number,Fixed, Date and UString.<br><small><span style="color:green">UString has been added since Ver.4.2.0</span></small>

### Relationship between image and text display position <br>
The relationship between the set image and the characters specified in the <a href="/package/standard/label/properties/value">Value</a>. property is as follows by specifying the <a href="/package/extension4/imagelabel/properties/vertplacement">VertPlacement</a> and <a href="/package/extension4/imagelabel/properties/horzplacement">HorzPlacement</a> properties.

<a href="/img/Package/Ext4-ImageLabel2.PNG" target="_blank">
<img src="/img/Package/Ext4-ImageLabel2.PNG" alt="login image"></a>

**Limitations when visual style is enabled**<br>
◆ Specifying the visual style is invalid.


**Precautions when scaling**<br>
  ◆ The image displayed internally is also subject to scaling.