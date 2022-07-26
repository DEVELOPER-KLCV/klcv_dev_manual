---
layout: default

grand_parent: 7. XML Package
parent: XmlNode Class
has_children: true
title: Properties
nav_order: 1
permalink: /package/xmlpackage/xmlnode/properties
has_toc: false
---
# {{ page.title }}

The following properties are defined in the XmlNode class.

|Name       | Access | Type   | Description |
|----------	|--------|--------|-------------|
| [Attributes](/package/xmlpackage/xmlnode/properties/attributes) | R | XmlNamedNodeMap |Attr node belonging to the node<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [ChildNodes](/package/xmlpackage/xmlnode/properties/childnodes) | R | XmlNodeList |Child node|
| [FirstChild](/package/xmlpackage/xmlnode/properties/firstchild) | R | XmlNode |First child node|
| [LastChild](/package/xmlpackage/xmlnode/properties/lastchild) | R | XmlNode |Last child node|
| [LocalName](/package/xmlpackage/xmlnode/properties/localname) | R | String |Node local name|
| [NamespaceURI](/package/xmlpackage/xmlnode/properties/namespaceuri) | R | String |Node namespace URI|
| [NextSibling](/package/xmlpackage/xmlnode/properties/nextsibling) | R | XmlNode |Next node|
| [NodeName](/package/xmlpackage/xmlnode/properties/nodename)* | R | String |Node name|
| [NodeType](/package/xmlpackage/xmlnode/properties/nodetype) | R | Integer |Node type|
| [NodeValue](/package/xmlpackage/xmlnode/properties/nodevalue) | CRW | String |Node value<br><small><span style="color:blue">In Mobile and AI only R can be accesed, cannot be initialized or changed.</span></small>|
| [OwnerDocument](/package/xmlpackage/xmlnode/properties/ownerdocument) | R | XmlDocument |Document node that is the top of the DOM tree to which the node belongs<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [ParentNode](/package/xmlpackage/xmlnode/properties/parentnode) | R | XmlNode |Parent node|
| [Prefix](/package/xmlpackage/xmlnode/properties/prefix) | CRW | String |Node namespace URI prefix<br><small><span style="color:blue">In Mobile and AI only R can be accesed, cannot be initialized or changed.</span></small>|
| [PreviousSibling](/package/xmlpackage/xmlnode/properties/previoussibling) | R | XmlNode |Previous node|
| [Text](/package/xmlpackage/xmlnode/properties/text) | R | String |Text that aggregates child nodes|
| [Xml](/package/xmlpackage/xmlnode/properties/xml) | R | String |XML text representing a node|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
