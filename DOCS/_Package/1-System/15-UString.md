---
layout: default

parent: 1. System Package
has_children: true

title: UString Class
nav_order: 15
permalink: /package/system/ustring

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class that holds Unicode strings. There is no limit to the length of the string that can be stored.

In the UString class, Unicode is used for the character code. Character strings are handled in character units.

However, the range that the UString class can handle is 2-byte Unicode. Please note that characters in the range larger than 2 bytes cannot be handled correctly.

The UString class can handle a wider range of characters than the [String](/package/system/string) class, and in the case of Japanese, it contains various characters that are not included in Shift_JIS, such as personal names and place names, and can be expressed in the original glyph form. ..

Comparisons and operations with String objects and string constants are automatically converted from Shift_JIS to Unicode. Also, if you assign a UString object to a String object or String type property, Unicode will be automatically converted to Shift_JIS.

When converting from Unicode to Shift_JIS, if a character that cannot be converted is detected, it is replaced with a "?" Mark. As a result, unintended consequences may occur, such as matching Unicode-specific characters with "?". Please be careful when handling character code conversion.

**<small>Not supported in Mobile, AI</small>**<br>
**<small>Supports Unicode strings in the String class for AI</small>**

<b>Default properties and ValueType</b>

The default property is [Value](). The ValueType specification is invalid.
