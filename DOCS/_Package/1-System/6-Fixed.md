---
layout: default

parent: 1. System Package
has_children: true

title: Fixed Class
nav_order: 6
permalink: /package/system/fixed

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class that holds fixed-point numbers.

Fixed classes are stored in 64-bit signed integer format with values ​​scaled by 10000. Internally, 1 is expressed as 10000 and 0.1 is expressed as 1000.

Unlike the [Number](/package/system/number) class, which holds internal data in floating-point format, errors due to floating-point characteristics do not occur in principle, but the range that can be expressed is limited to 15 digits for the integer part and 4 digits for the decimal part. .. If the operation result exceeds the expression range, the integer part is rounded down from the one with the larger digit position, and the decimal part is rounded down from the 5th place or less.

If you pass an operation between a Fixed class and a class of other types, or a Fixed class to a method or function that receives a number, the calculation will be performed automatically based on the result of conversion to Number type. Therefore, in such a case, it behaves as a floating point number.

<b>Default properties and ValueType</b>
 
The default property is [Value](/package/system/fixed/properties/value). The ValueType specification is invalid.