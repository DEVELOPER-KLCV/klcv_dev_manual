---
layout: default

parent: 1. System Package
has_children: true

title: Array
nav_order: 1
permalink: /package/system/Array

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---
A class that holds a dynamic array.

CRS programs can handle arrays in two ways: the Array class and [array objects](/bizBrowserV/6/6-1/).

The Array class does not require you to specify a specific type for each element, and each element can store values ​​such as objects, numbers, and strings that have different types.

The Array class, unlike array objects, automatically expands the number of elements.

You can access elements with subscripts with "[]", but you can also use letters as subscripts instead of numbers. (Associative array)

Note that the behavior is different between an associative array that uses a string as a subscript and an array that uses a number. If the subscript is a number, it can be sorted, but it cannot be sorted in an associative array.

<b>Default properties and ValueType</b>

The default property is [Value](/package/system/array/properties/value). The ValueType specification is invalid.