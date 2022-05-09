---
layout: default

grand_parent: Object Class
parent: Properties
has_children: false
title: Object.Length property
nav_order: 6
permalink: /package/system/object/properties/length
---
# {{ page.title }}

A property attached only to array objects that represents the number of elements in the array.

 

This property is attached to the array object. Note that it is not attached to individual array elements.

 
```
Number num [3];
MessageBox (num.Length);     / * 3 is displayed in this line * /
MessageBox (num [1] .Length); / * This line is an error. Length is not added to the element * /
```

This property has no effect on non-arrayed objects.

 

This property is read-only and cannot be updated.