---
layout: default

grand_parent: 7. XML Package
parent: XmlDocument Class
has_children: true
title: Properties
nav_order: 1
permalink: /package/xmlpackage/xmldocument/properties
has_toc: false
---
# {{ page.title }}

The following properties are defined in the XmlDocument class.

|Name       | Access | Type   | Description |
|----------	|--------|--------|-------------|
| [DocType](/package/xmlpackage/xmldocument/properties/doctype) | R | XmlDocumentType |DocumentType node<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [DocumentElement](/package/xmlpackage/xmldocument/properties/documentelement) | R | XmlElement |Element node at the beginning of the document|
| [DocumentURI](/package/xmlpackage/xmldocument/properties/documenturi) | CRW | String |URL from which the CRS was obtained<br><small><span style="color:red">Added since Ver.4.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [Implementation](/package/xmlpackage/xmldocument/properties/implementation) | R | XmlDOMImplementation |This Document node is created<br>XmlDOMImplementation object<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [IndexAttributeName](/package/xmlpackage/xmldocument/properties/indexattributename) | CRW | String |The name of the ID attribute used in the GetElementById method<br><small><span style="color:red">Added since Ver.4.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable