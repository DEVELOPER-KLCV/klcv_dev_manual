---
layout: default

parent: 1. System Package
has_children: true

title: String Class
nav_order: 14
permalink: /package/system/string

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class that holds strings. There is no limit to the length of the string that can be stored.

<b>About String class in PC version and Mobile version</b>

In the String class, Shift_JIS is used for the character code. The character string is handled in 1-byte units.

If a character that cannot be converted to Shift_JIS is detected in the data obtained from XML that handles Unicode, it will be replaced with a "?" Mark. (Unicode can be handled by UString class)

<b>About String class in Android version</b>

Unicode is used for the character code in the String class in the Android version. Even double-byte characters are handled in single character units.

Therefore, the description of the property and the usage of the method (handling of the number of characters) are the same as the property and method of the UString class. See the description of the UString class.

<b>Default properties and ValueType</b>
 
The default property is [Value](/package/system/string/properties/value). The ValueType specification is invalid.