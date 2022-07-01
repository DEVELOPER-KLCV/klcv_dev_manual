---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ListView Class
nav_order: 11
permalink: /package/extension4/listview

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ListView.PNG" target="_blank">
<img src="/img/Package/Ext4-ListView.PNG" alt="login image"></a>

A class that displays a list view. The list view has functions to display in multiple formats such as icon display and list display.

The ListView class works in conjunction with the <a href="/package/extension4/listviewitem">ListViewItem</a>, <a href="/package/extension4/listviewsubitem">ListViewSubItem</a>, and <a href="/package/extension4/listviewheader">ListViewHeader</a> classes.

To set the data to be displayed as an item, you need to place the ListViewItem class or its derived class objects in the structure defined under the ListView object.

**Screen Display Example**

ListStyle = $REPORT
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listview.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

ListStyle = $LIST
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listview.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

ListStyle = $SMALLICON
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listview.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

ListStyle = $LARGEICON
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_listview.files/image004.png" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>

**Printer output by Doc class**<br>
Not subject to printing.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/listview/properties/value">Value</a>. The ValueType specification is invalid.

### Icon specification<br>
The types of icons displayed are as follows by default.

<a href="/img/Package/Ext4-ListView1.PNG" target="_blank">
<img src="/img/Package/Ext4-ListView1.PNG" alt="login image"></a>

You can also use the SetImage method to change to the icon stored in the ImageList object.

**Restrictions when visual style is enabled**<br>
Nothing in particular


**Precautions when scaling**<br>
◆ The line height when displaying the report depends on the icon size and font size.