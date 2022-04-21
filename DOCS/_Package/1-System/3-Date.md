---
layout: default

parent: 1. System Package
has_children: true

title: Date Class
nav_order: 3
permalink: /package/system/date

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class that holds dates and times.

The date is represented by a real number with 1900/1/1 as 1.0, the interval of one day is 1.0, and the interval of one second is 1 / 86,400. The disassembly accuracy is 1 second.

The valid range of the Date class is from January 1, 1900 to December 31, 2099. If you specify a number that exceeds the range, the date will be undefined.

<b>Default properties and ValueType</b>

The default property is [Value](/package/system/date/properties/value). The ValueType specification is invalid.