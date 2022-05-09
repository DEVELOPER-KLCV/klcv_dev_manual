---
layout: default

grand_parent: Object Class
parent: Properties
has_children: false
title: Object.ValueType property
nav_order: 4
permalink: /package/system/object/properties/valuetype
---
# {{ page.title }}

  *ValueType is not strictly a property, but it is treated as a property here for convenience. <br><br>

 

ValueType represents the data type of the object. ValueType is specified in the following format.

ClassName: ValueType Name

Example
```
TextBox: Number TextBox1 {
    ...
}
```

The above example defines a textbox with a data type of Number .

Value Type can be omitted. If ValueType is omitted in a class that can be specified like the TextBox class, it will be a String type.

```
TextBox TextBox1 {
    / * Default ValueType is String * /
}
```

Some object data types are fixed by class. For example, the DateEdit class is always of type Date , so specifying ValueType is invalid.

 

ValueType is also the data type of the default property because the default property of each class represents the value of the object .

 

The type of data type that can be specified for ValueType depends on the class specifications. See the description of each class for details.

 

ValueType can be set like a property in the property view in Biz / Designer, but since it is not strictly a property, the following cannot be specified in the CRS script.

```
TextBox TextBox1 {
    ValueType = Number; / * Example of incorrect specification * /
}
```

<small>UString cannot be specified for Value Type in Mobile & AI</small>
