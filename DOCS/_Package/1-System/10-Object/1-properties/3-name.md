---
layout: default

grand_parent: Object Class
parent: Properties
has_children: false
title: Object.Name property
nav_order: 3
permalink: /package/system/object/properties/name
---
# {{ page.title }}

Indicates the name of the object as a string. The name of the object is the name identified in the object tree.

CRS allows you to access an object by multiple names by storing the object reference in the var variable. The Name property indicates the name given to the object when it is connected to the object tree, regardless of the name (label) of these var variables. The Name property of an object that is not connected to the object tree is usually an empty string and unnamed.

The object name is specified in a regular object tree connection statement or in the [Append](/package/system/object/methods/append) method.

Object tree connection statement example

```
Form form1 {
     :
    Button Button1 {
        :
    }
     :
}
```

In this example, form1 and button1 are stored in the Name property.

Append example

```
:
var obj = new String;
Append(obj, "StringA");
:
```

In this example, StringA is stored in the Name property.

This property is read-only and cannot be updated.