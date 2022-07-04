---
layout: default

parent: 4. Extension4 Package
has_children: true

title: SplitterForm Class
nav_order: 17
permalink: /package/extension4/splitterform

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-SplitterForm.PNG" target="_blank">
<img src="/img/Package/Ext4-SplitterForm.PNG" alt="login image"></a>

A class that defines each form of the <a href="/package/extension4/splitterframe">SplitterFrame</a> class. Be sure to use it as a child object of the SplitterFrame class.

The SplitterForm class has no specific functionality and can be placed under the SplitterFrame object and used in much the same way as the <a href="/package/standard/form">Form</a> class.

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/form/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>

**Restrictions when visual style is enabled**<br>
Nothing in particular

**Precautions when scaling**<br>
Nothing in particular