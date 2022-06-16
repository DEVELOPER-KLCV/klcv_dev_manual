---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ComboBox Class
nav_order: 1
permalink: /package/extension4/combobox

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ComboBox.PNG" target="_blank">
<img src="/img/Package/Ext4-ComboBox.PNG" alt="login image"></a>

A class that displays a combo box. It looks similar to the <a href="/package/standard/pulldownlist">PulldownList</a> class, but you can type characters from the keyboard as well as select from the options.

The ComboBox class works in tandem with the <a href="/package/extension4/comboitem">ComboItem</a> class.
To set the data to be displayed as choices, you need to place the ComboItem class or its derived class objects in the structure defined under the ComboBox object.


**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_combob.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Printer output by Doc class**<br>
 Not subject to printing.


**Default properties and ValueType**<br>
  The default property is <a href="/package/extension4/combobox/properties/value">Value</a> . ValueType can be String and UString.<br><small><span style="color:green">Value Type can be specified since Ver.5.0.3</span></small><br><br>

 
**Restrictions when visual style is enabled**<br>
 Nothing in particular


 **Precautions when scaling**<br>
◆ The apparent height (height that is not pulled down) is not affected by VerticalScale, but is affected by font size changes by FontScale.
◆ The width of the pull-down button is specified by the OS and is not subject to scaling.