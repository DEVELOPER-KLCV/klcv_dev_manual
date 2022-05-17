---
layout: default

parent: 2. Standard Package
has_children: true

title: Dialog Class
nav_order: 5
permalink: /package/standard/dialog

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std20.files/image001.gif" %}

# {{ page.title }}

<a href="/img/Package/Standard-Dialog.PNG" target="blank"><img src="/img/Package/Standard-Dialog.PNG" alt="Standard-Dialog"></a>

A class that displays a dialog.

Dialogs are application modal and you cannot interact with other windows until you close them.

 

Only one <a href="/package/standard/form">Form</a> object can be created as a child object in a Dialog object. Create other display objects as child objects of the Form object rather than directly under the Dialog object.

 

Dialog objects belong to the hierarchy as child objects of other display objects, but they appear as visually separate windows.

 

**Screen display example**

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**

Form objects represent areas on paper. Unlike when displayed on the screen, printing is performed without clipping even if the child object is located at a position beyond the display range of the Form object.

**Default properties and ValueType**

The default property is Value. ValueType can be String, Number, Fixed, Date, UString.<br>
<small><span  style="color:green">UString has been added from Ver.4.2.0</span ></small>

<b>Restrictions when visual style is enabled</b>

Nothing in particular