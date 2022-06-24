---
layout: default

parent: 4. Extension4 Package
has_children: true

title: GroupBox Class
nav_order: 6
permalink: /package/extension4/groupbox

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-GroupBox.PNG" target="_blank">
<img src="/img/Package/Ext4-GroupBox.PNG" alt="login image"></a>

A class that displays a group box.

The position of the displayed title (top, bottom, left, right) can be set with the TitilePosition property.

If there is no title, the frame will be drawn in the same size as the display range.

Box type and line type display is possible.

**Screen Display Example**

BoxStyle = $BOX <br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_groupbox.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

---

BoxStyle = $BOX <br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_groupbox.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

---

BoxStyle = $BOX <br>
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_groupbox.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

---

BoxStyle = $BOX <br>
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_groupbox.files/image004.png" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>

**Box Type Title Display**<br>
If you specify $BOX or $ROUND for the <a href="/package/extension4/groupbox/properties/boxstyle">BoxStyle</a> property, the box type display will be displayed.

Normally, the title overlaps the border, but in $SUNKEN, $RISED, $SOFTBUMP, $FLATSUNKEN, and $FLATRISED, it appears outside the border.

**Line Type Title Display**<br>
If you specify $HORZLINE or $VERTLINE for the <a href="/package/extension4/groupbox/properties/boxstyle">BoxStyle</a> property, the line type display will be displayed.

The title usually overlaps the line, but if the <a href="/package/extension4/groupbox/properties/borderstyle">BorderStyle</a> property is $SUNKEN, $RISED, $SOFTBUMP, $FLATSUNKEN, $FLATRISED, it will appear above or below the line (left or right for $ VERTLINE). The display position at this time can be specified by the <a href="/package/extension4/groupbox/properties/titleposition">TitlePosition</a> property $TOP and $BOTTOM ($LEFTSIDE and $RIGHTSIDE in $VERTLINE).

**Printer output by Doc class**<br>
It will be printed in the same way as the screen.

The ruled line is a solid line, but it is printed according to the style only when the <a href="/package/extension4/groupbox/properties/borderstyle">BorderStyle</a>  property is set to $DASH or $DOT.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/combobox/properties/value">Value</a> . ValueType can be String and UString.<br><small><span style="color:green">Value Type can be specified since Ver.5.0.3</span></small><br>

 
**Restrictions when visual style is enabled**<br>
◆ Visual style specification is invalid


**Precautions when scaling**<br>
Nothing in particular