---
layout: default

parent: 7. XML Package
has_children: true

title: XmlNode Class
nav_order: 11
permalink: /package/xmlpackage/xmlnode

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

The base class for all nodes. It has the basic functionality of the nodes that make up the DOM tree.

The XmlNode class is a virtual class and cannot instantiate itself.

Classes derived from the XmlNode class inherit the properties and methods defined in the XmlNode class and can be used in the same way. 

For classes derived from XmlNode, there is :<br>

[XmlDocumentFragment](/package/xmlpackage/xmldocumentfragment)<br>
[XmlDocument](/package/xmlpackage/xmldocument)<br>
[XmlAttr](/package/xmlpackage/xmlattr)<br>
[XmlElement](/package/xmlpackage/xmlelement)<br>
[XmlCharacterData](/package/xmlpackage/xmlcharacterdata)<br>
[XmlText](/package/xmlpackage/xmltext)<br>
[XmlCDATASection](/package/xmlpackage/xmlcdatasection)<br>
[XmlComment](/package/xmlpackage/xmlcomment)<br>
[XmlProcessingInstruction](/package/xmlpackage/xmlprocessinginstruction).

In Mobile and Android versions, XmlNode has a different meaning, and all nodes other than XmlDocument, XmlElement, and XmlText are instantiated as XmlNode objects.

**Default properties and ValueType**

The default property is [NodeName](/package/xmlpackage/xmlnode/properties/NodeName). The ValueType specification is invalid.