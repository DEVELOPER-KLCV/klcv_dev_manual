---
layout: default

parent: 2. Standard Package
has_children: true

title: EditBox Class
nav_order: 8
permalink: /package/standard/editbox

---

# {{ page.title }}

<a href="/img/Package/Standard-Editbox.PNG" target="_blank">
<img src="/img/Package/Standard-Editbox.PNG" alt="login image">
</a>

A class that displays a multi-line input edit box.


The character to be displayed is the value of the <a href="/package/standard/editbox/properties/value">Value</a> property. String, Number, Fixed, Date, and UString can be specified for<a href="/package/system/object/properties/valuetype">ValueType</a>, but two types, String and UString, are useful for the purpose of using the edit box.


In the String type specification, the internal character code is a platform-dependent multi-byte character code (Shift-JIS in the Japanese environment).

In the UString type, the internal character code is Unicode, which makes it possible to handle a wider variety of characters.

In Windows98 and ME, the Unicode input function at the OS level is not supported, so Unicode-specific characters cannot be input or displayed, and cannot be specified together with the <a href="/package/standard/editbox/properties/maxlength">MaxLength</a> property.

<small><span style="color:green">Since Ver.5.0.0, it is possible to use the Insert key to switch between insert mode and overwrite mode.</span></small>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std4.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Printer output by Doc class**<br>
Enclose the characters in a rectangle and display them.

Even if the UString type is specified, all characters are converted to multibyte when printing, so Unicode -specific characters are printed as "?".

**Default properties and ValueType**<br>

The default property is Value. ValueType can be String , Number , Fixed , Date , UString

<small><span style="color:green">UString has been added since Ver.4.2.0</span></small>


**Restrictions when visual style is enabled**<br>

 

Nothing in particular

 

**Precautions when scaling**<br>

 

Nothing in particular