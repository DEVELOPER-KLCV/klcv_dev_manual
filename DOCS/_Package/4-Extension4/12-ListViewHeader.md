---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ListViewHeader Class
nav_order: 12
permalink: /package/extension4/listviewheader

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ListViewHeader.PNG" target="_blank">
<img src="/img/Package/Ext4-ListViewHeader.PNG" alt="login image"></a>

This class is for manipulating the column header of the <a href="/package/extension4/listview">ListView</a> class.

The <a href="/package/extension4/listview/methods/getheader">ListView.GetHeader</a> method creates a ListViewHeader object and allows you to set the column headers. Column headers are only valid if the <a href="/package/extension4/listview/properties/liststyle">ListView.ListStyle</a> property is $REPORT (report format).

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/label/properties/value">Value</a>. ValueType can be String,Number,Fixed and Date.

















