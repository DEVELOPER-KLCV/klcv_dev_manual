---
layout: default

parent: 6. CSV Package
has_children: true

title: CSVDocument Class
nav_order: 1
permalink: /package/csvpackage/csvdocument

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that holds CSV data.

The CSVDocument class has the following features.

1. All cell data is stored in one CSVDocument object and it is lightweight.
1. You can freely add or delete rows and columns.
1. Sorting, merging, and file input / output are possible.

<b>Default properties and ValueType</b>

The default property is [Value](/package/csvpackage/csvdocument/properties/Value). ValueType can be String, Number, Fixed, Date, UString.
If ValueType is specified for UString, the internal character code will be Unicode.
This is synonymous with specifying Unicode as the internal character code in the constructor.<br>
**<small>Added since Version 5.0.3</small>**