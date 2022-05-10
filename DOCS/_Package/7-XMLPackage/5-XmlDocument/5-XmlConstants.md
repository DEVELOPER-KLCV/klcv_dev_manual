---
layout: default

grand_parent: 7. XML Package
parent: XmlDocument Class
has_children: true
title: XML Constants
nav_order: 5
permalink: /package/xmlpackage/xmldocument/constants
has_toc: false
---
# {{ page.title }}

The XML package defines XML constants. XML constants can be used by the << operator to populate the [XmlDocument](/package/xmlpackage/xmldocument) object.

Within the XML constant block, there is no grammatical relevance to the CRS script, so CRS syntax (such as enclosing strings in ""), constants (such as $RED), operators (such as + and-), and functions. Etc. cannot be used. You have to follow the format as XML.

You can write the XML data directly in the CRS script in the following format.

```
xml <<-
（XMLデータ）
->>;
```

Use Example
```
var x = new XmlDocument();
x << xml <<-
<?xml version="1.0" encoding="SHIFT_JIS"?>
<data>
    <record title="Record１">
        <item1>Item １</item1>
        <item2>Item １</item2>
        <item3>Item １</item3>
    </record>
</data>
->>;
```