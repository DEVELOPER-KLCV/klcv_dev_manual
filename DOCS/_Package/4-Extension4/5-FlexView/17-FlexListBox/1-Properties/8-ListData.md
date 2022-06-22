---
layout: default

grand_parent: FlexListBox Class
parent: Properties
has_children: false
title: FlexListBox.ListData Property
nav_order: 8
permalink: /package/extension4/flexview/flexlistbox/properties/listdata
---
# {{ page.title }}

Specifies the options displayed in the list box.

If specify UString for ValueType, this property behaves as a UString type.
<br><small><span style="color:red">Added since Ver.5.0.3</span></small>

The options are specified as comma-separated strings. It cannot contain line breaks or tabs.

If want to include a comma in the options, enclose one element in double-coating (") or escape it with \.

If want to include double coating (") in the options, write double coating (") instead of enclosing one element in double coating (")" or escape with \.

Specification example

```
FlexListBox1.ListData = "選択肢1,選択肢2,選択肢3";
FlexListBox2.ListData = "\"1,000\",\"2,000\",\"3,000\"";
FlexListBox3.ListData = "1\\,売上,2\\,仕入,3\\,破棄";
```


Display example

ListData = "選択肢1,選択肢2,選択肢3" <br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlistboxp1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

ListData = "\"1,000\",\"2,000\",\"3,000\""<br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlistboxp1.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>


ListData = "1\\,売上,2\\,仕入,3\\,破棄"<br>
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlistboxp1.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>