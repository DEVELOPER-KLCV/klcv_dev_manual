---
layout: default

grand_parent: 17. JSON Package
has_children: true

parent: JSONDocument Class
has_children: true
title: JSON Constants
nav_order: 5
permalink: /package/jsonpackage/jsondocument/constants
has_toc: false
---
# {{ page.title }}

The JSON package defines JSON constants. JSON constants can be used by the << operator to populate the [JSONDocument](/package/jsonpackage/jsondocument) object.

CRS syntax, constants (such as $RED), operators (such as + and-), functions, etc. cannot be used inside JSON constant blocks because they are not grammatically related to CRS scripts. You have to follow the format as JSON.

You can write JSON data directly in the CRS script in the following format.

```
json <<-
（JSON data）
->>;
```

Use Example
```
var j = new JSONDocument();
j << json <<-
{
    "data": [
        {
            "title": "Record １",
            "item1": "Item １",
            "item2": "Item １",
            "item3": "Item １"
        }
    ]
}
->>;
```