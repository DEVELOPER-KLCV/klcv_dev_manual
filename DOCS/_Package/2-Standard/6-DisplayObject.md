---
layout: default

parent: 2. Standard Package
has_children: true

title: DisplayObject Class
nav_order: 6
permalink: /package/standard/displayobject

---


# {{ page.title }}

<a href="/img/Package/Standard-Display.PNG" target="blank"><img src="/img/Package/Standard-Display.PNG" alt="Standard-Display"></a>

This is the base class for the screen display class. It has the basic functions of screen display, and all screen display classes are derived from the DisplayObject class.<br><br>

The DisplayObject-derived class should place the object as part of an object tree that starts with "//" (<a href="/package/standard/root">Root</a> object).<br>

You cannot create an instance without being connected to the object tree with the new operator, or place it in the global namespace with import. <br><br>

Also, only objects derived from the <a href="/package/standard/containerobject">ContainerObject</a> class are allowed as parent objects in the object tree. Objects that are not derived from the ContainerObject class, such as String and Date, cannot be created as parents.<br><br>

The DisplayObject class is a virtual class and cannot instantiate itself.<br><br>

In the Mobile version, the DisplayObject class does not exist because there is no concept of class, but in the explanation of common properties and methods, it is explained as DisplayObject class for convenience.