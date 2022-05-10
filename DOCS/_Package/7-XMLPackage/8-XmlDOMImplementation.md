---
layout: default

parent: 7. XML Package
has_children: true

title: XmlDOMImplementation Class
nav_order: 8
permalink: /package/xmlpackage/xmldomimplementation

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that defines the implementation of the DOM.

It manages the creation of the [XmlDocument](/package/xmlpackage/xmldocument) object that is the root node of the DOM tree and the corresponding version of the DOM API.

**Default properties and ValueType**
 
The default property is [Value](/package/xmlpackage/xmldomimplementation/properties/value). ValueType can be String, Number, Fixed, Date, UString.
If ValueType is specified for UString, the internal character code will be Unicode.
This is synonymous with specifying Unicode as the internal character code in the constructor.

<br>
**<small>Added since Version 5.0.3</small>**