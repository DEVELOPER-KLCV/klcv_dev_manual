---
layout: default

grand_parent: Object Class
parent: Properties
has_children: false
title: Object.Index property
nav_order: 5
permalink: /package/system/object/properties/_index
---
# {{ page.title }}

A property attached only to an array element object, which indicates the position (subscript) of the array element.

 

This property is attached to each array element. Note that it is not attached to the array object.

 
```
Number num [3];
MessageBox (num [1] .Index); / * 1 is displayed in this line * /
MessageBox (num.Index);     / * This line is an error. Index is not added to the array object * /
``` 

This property has no effect on non-arrayed objects.

 

This property is read-only and cannot be updated.