---
layout: default

parent: 7. XML Package
has_children: true

title: XmlProcessingInstruction Class
nav_order: 13
permalink: /package/xmlpackage/XmlProcessingInstruction

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---
<a href="/img/Package/XML-XmlProcessingInstructionClass.png" target="_blank">
<img src="/img/Package/XML-XmlProcessingInstructionClass.png" alt="login image"></a>

A class that defines a Processing Instruction node.

The XML prologue (<? Xml version = "1.0"?> Part) is also a processing instruction in XML syntax, but because it is processed specially, the corresponding Processing Instruction node is not generated. Also, if you refer to the XML source with the [XmlNode.Xml](/package/xmlpackage/xmlnode/properties/xml) property, which is a specification specific to Biz / Browser, the prologue part will be added automatically. Therefore, when outputting XML to a file etc., it is not necessary to add a Processing Instruction node for prologue.

If you want to include your own processing instructions as part of the DOM tree, create an XmlProcessingInstruction object with the [XmlDocument.CreateProcessingInstruction](/package/xmlpackage/xmldocument/methods/createprocessinginstruction) method and connect to the DOM tree with methods such as [XmlNode.AppendChild](/package/xmlpackage/xmlnode/methods/appendchild), [XmlNode.InsertBefore](/package/xmlpackage/xmlnode/methods/insertbefore), and [XmlNode.ReplaceChild](/package/xmlpackage/xmlnode/methods/replacechild).

**Default properties and ValueType**

The default property is [NodeName](/package/xmlpackage/xmlnode/properties/NodeName). The ValueType specification is invalid.