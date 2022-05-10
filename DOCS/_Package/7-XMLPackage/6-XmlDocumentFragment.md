---
layout: default

parent: 7. XML Package
has_children: true

title: XmlDocumentFragment Class
nav_order: 6
permalink: /package/xmlpackage/xmldocumentfragment

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that maintains a fragment of a document.

The DOM tree is built under the Document node, but if you want to make major changes to the tree structure, it would be efficient if you could temporarily build the tree in a location other than the Document node. The XmlDocumentFragment class can act as the root element of the DOM tree instead of the [XmlDocument](/package/xmlpackage/xmldocument) class in these cases.

The XmlDocumentFragment class itself only functions as a placeholder and does not hold XML data like other nodes. Therefore, you cannot reference or set data on the XmlDocumentFragment object.
The XmlDocumentFragment class inherits all properties and methods from the XmlNode class. No unique properties or methods are defined, but properties or methods that reference or manipulate XML data are invalid for the reasons described above.

**Default properties and ValueType**

The default property is [NodeName](/package/xmlpackage/xmlnode/properties/NodeName). The ValueType specification is invalid.