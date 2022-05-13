---
layout: default

parent:  17. JSON Package
has_children: true

title: JSONDocument Class
nav_order: 1
permalink: /package/jsonpackage/jsondocument

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that parses and outputs JSON data.

The JSON data loaded by the [Get](/package/jsonpackage/jsondocument/methods/get), [Load](/package/jsonpackage/jsondocument/methods/load), or [Parse](/package/jsonpackage/jsondocument/methods/parse) method is expanded to the Array object, and the first Array object is set to Value.

Also, the [Save](/package/jsonpackage/jsondocument/methods/save) method converts the Array object set in Value to JSON data.

**JSON-Array conversion rule**
The array enclosed in [] is expanded as the 0th array of Array, and the object enclosed in {} is expanded as an associative array of Array with the name as the key.
Objects and arrays as values ​​are in the form of Array stored in the elements of Array.

**Example**


<a href="/img/Biz Browser V/JSONData.PNG" target="_blank">

<img src="/img/Biz Browser V/JSONData.PNG" alt="json data image">


**Default properties and ValueType**
 
The default property is [Value](/package/jsonpackage/jsondocument/properties/value). ValueType can be String, Number, Fixed, Date, UString.