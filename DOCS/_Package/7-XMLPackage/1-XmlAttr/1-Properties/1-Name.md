---
layout: default

grand_parent: XmlAttr Class
parent: Properties
has_children: false
title: XmlAttr.Name property
nav_order: 1
permalink: /package/xmlpackage/xmlattr/properties/name
---
# {{ page.title }}

The attribute name of the Attr node.

**<small>Add more from here ---></small>**

**Unicode-specific character constraints**

Since the Name property is implemented by the [Name](/package/system/object/properties/name) property defined by the [Object](/package/system/object) class, the character code is fixed to the multibyte character code (Shift-JIS in the case of Japanese environment) even if [the internal character code is Unicode](/package/xmlpackage/xmldomimplementation/methods/constructor). increase. Therefore, if Unicode-specific characters are set in the Name property, they will not be processed correctly.<br>
**<small><--- Up to here</small>**

This property is read-only and cannot be changed.
