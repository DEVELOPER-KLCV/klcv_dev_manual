---
layout: default

parent: 4. Extension4 Package
has_children: true

title: MaskEdit Class
nav_order: 15
permalink: /package/extension4/maskedit

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-MaskEdit.PNG" target="_blank">
<img src="/img/Package/Ext4-MaskEdit.PNG" alt="login image"></a>

A class that displays mask edits.

Mask Edit is a text box for inputting a fixed-length character string whose input format and output format can be customized by specifying the <a href="/package/extension4/maskedit/properties/mask">Mask</a> property.

If the Mask property is not specified, the operability will be the same as for the <a href="/package/standard/textbox">TextBox</a> class.

The MaskEdit class cannot check the relevance of each input field. For example, the relevance of the date. Use the <a href="/package/extension3/datedit">DateEdit</a> class if you need to enter the exact date, and the <a href="/package/extension3/numberedit">NumberEdit</a> class if you need to enter the exact number.

When the entered value is confirmed, the following properties will be updated according to the input status.

<a href="/package/extension4/maskedit/properties/value">Value</a> property<br>
If the input value meets the specifications of the Mask property, it will be updated with the input value. If the Mask property specification is not met, it will be updated to an empty string. As a result, a Touch event is fired if the Value property changes from what it was before. Also, the Change event is fired if the UseChange property is set to $TRUE.

<a href="/package/extension4/maskedit/properties/edittext">EditText</a> property<br>
It will be updated to the character string displayed on the screen.

<a href="/package/extension4/maskedit/properties/invalidtext">InvalidText</a> property<br>
If the input value meets the specifications of the Mask property, it will be updated to $FALSE. If the Mask property specification is not met, it will be updated to $TRUE.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_maskedit.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
It will be printed in the same way as the screen.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/listview/properties/value">Value</a>. The ValueType specification is invalid.

**Restrictions when visual style is enabled**<br>
Nothing in particular

**Precautions when scaling**<br>
Nothing in particular
