---
layout: default

parent: 7. XML Package
has_children: true

title: XmlAttr Class
nav_order: 1
permalink: /package/xmlpackage/xmlattr

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that defines an Attr node. Since the Attr node does not belong to the DOM tree, the XmlAttr class is derived from the XmlNode class, but properties such as [ParentNode](/package/xmlpackage/xmlnode/properties/parentnode), [PreviousSibling](/package/xmlpackage/xmlnode/properties/previoussibling), and [NextSibling](/package/xmlpackage/xmlnode/properties/nextsibling) are null.

**Default properties and ValueType**

The default property is [NodeName](/package/xmlpackage/xmlnode/properties/NodeName). The ValueType specification is invalid.