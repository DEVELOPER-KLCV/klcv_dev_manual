---
layout: default

parent: 2. Standard Package
has_children: true

title: EditObject Class
nav_order: 9
permalink: /package/standard/editobject

---


# {{ page.title }}

<a href="/img/Package/Standard-EditObject.PNG" target="_blank">
<img src="/img/Package/Standard-EditObject.PNG" alt="login image">
</a>


The base class of the character input class. There is a basic function of character editing processing with the keyboard.


The EditObject class is a virtual class and cannot instantiate itself.

If you assign binary data that is not considered as a string to the derived class of EditObject, the display will be undefined.

 

In the Mobile version, there is no EditObject class because there is no concept of class, but in the explanation of common properties and methods, it is explained as EditObject class for convenience.



### Timing the Value Property Updated

In the EditObject derived class, the input value on the screen is stored in the Value property, but the actual change of the Value property is triggered by the following.

1. When an object loses keyboard focus

2. When you press Enter or F1 to F12

3. When selecting from the combo box dropdown (<a href="/package/extension4/combobox">ComboBox</a> class)

Therefore, please note that you cannot get the data in progress even if you refer to the Value property of the object in the event handler that does not involve the focus movement, such as the <a href="/package/standard/displayobject/events/timer">Timer</a> event and the <a href="/base/clicked">Clicked</a> event of the <a href="/package/standard/label">Label</a> class. If you need to get the data being input in such a situation, call the <a href="/package/standard/root/methods/decidevalue">DecideValue</a> method of the <a href="/package/standard/root">Root</a> class before referencing the Value property, and reflect the value on the screen in the Value property.