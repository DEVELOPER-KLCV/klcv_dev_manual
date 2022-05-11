---
layout: default

grand_parent: JSONDocument Class
parent: Operators
has_children: false
title: JSONDocument << JSON Constants Operator
nav_order: 1
permalink: /package/jsonpackage/jsondocument/operators/1
---
# {{ page.title }}

This operator loads the [JSON constants](/package/jsonpackage/jsondocument/constants) on the right side of the JSONDocument object on the left side.

Example of use

```
var j = new JSONDocument();
j << json <<-
{
    "data": [
        {
            "title": "レコード１",
            "item1": "アイテム１",
            "item2": "アイテム１",
            "item3": "アイテム１"
        }
    ]
}
->>;
```