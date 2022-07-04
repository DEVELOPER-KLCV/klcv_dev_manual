---
layout: default

parent: 4. Extension4 Package
has_children: true

title: TextFrame Class
nav_order: 20
permalink: /package/extension4/textframe

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-TextFrame.PNG" target="_blank">
<img src="/img/Package/Ext4-TextFrame.PNG" alt="login image"></a>

A class that displays a read-only multi-line display edit box. Use this when you want to display multi-line character data in an area with a scroll bar.

It looks similar to the <a href="/package/standard/editbox">EditBox</a> class, but the user cannot enter or edit the editbox. If you use the EditBox class with non-editable settings, the background will be gray, but with the TextFrame class you can use it as it is.

Also, if you set the <a href="/package/standard/displayobject/properties/active">Active</a> property to $FALSE, you can display it as an object that does not receive focus (without becoming inactive) as it looks.

The character to be displayed is the value of the  <a href="/package/extension4/textframe/property/value">Value</a> property. String, Number, Fixed, Date, and UString can be specified for <a href="/package/system/object/properties/valuetype">ValueType</a>, but two types, String and UString, are useful for the purpose of using the edit box.

In the String type specification, the internal character code is a platform-dependent multi-byte character code (Shift-JIS in the Japanese language environment).

In the UString type, the internal character code is Unicode, which makes it possible to handle a wider variety of characters.

In Windows98 and ME, the Unicode input function at the OS level is not supported, so it is not possible to input or display Unicode-specific characters.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_textframe.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
Enclose the characters in a square and display them.

Even if the UString type is specified, all characters are converted to multibyte when printing, so Unicode-specific characters are printed as "?".

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/textframe/property/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>

**Restrictions when visual style is enabled**<br>
Nothing in particular

**Precautions when scaling**<br>
Nothing in particular