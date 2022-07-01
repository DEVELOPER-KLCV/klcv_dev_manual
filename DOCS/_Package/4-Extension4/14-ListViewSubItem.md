---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ListViewSubItem Class
nav_order: 14
permalink: /package/extension4/listviewsubitem

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ListViewSubItem.PNG" target="_blank">
<img src="/img/Package/Ext4-ListViewSubItem.PNG" alt="login image"></a>

A class that defines each subitem of the <a href="/package/extension4/listviewitem">ListViewItem</a> class. Be sure to use it as a child object of the ListViewItem class.


Only valid if the <a href="/package/extension4/listview/properties/liststyle">ListView.ListStyle</a> property is $REPORT (report format). The leftmost column is defined by the ListViewItem class, and the subsequent columns are defined by the ListViewSubItem class.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listviewsubitem.files/image001.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/label/properties/value">Value</a>. ValueType can be String, Number, Fixed and Date.