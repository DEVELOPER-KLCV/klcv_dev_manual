---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ListViewItem Class
nav_order: 13
permalink: /package/extension4/listviewitem

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ListViewItem.PNG" target="_blank">
<img src="/img/Package/Ext4-ListViewItem.PNG" alt="login image"></a>

A class that defines each item in the <a href="/package/extension4/listview">ListView</a> class. Be sure to use it as an array as a child object of the ListView class.

If the <a href="/package/extension4/listview/properties/liststyle">ListView.ListStyle</a> property is $REPORT (report format), the ListViewItem class corresponds to the leftmost column and also defines the entire row. (Other columns are defined in the <a href="/package/extension4/listviewsubitem">ListViewSubItem</a> class)

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listviewitem.files/image001.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Default properties and ValueType**<br>
The default property is <a href="/package/standard/label/properties/value">Value</a>. ValueType can be String, Number, Fixed and Date.