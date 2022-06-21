---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.TitleHorzAlign Property
nav_order: 4
permalink: /package/extension4/flexview/flexitem/properties/titlehorzalign
---
# {{ page.title }}

Specifies the horizontal layout of column titles.

In addition to the TitleHorzAlign property, title assignments are also affected by the HorizontalAlign property defined by FlexLabel, FlexTextBox, and so on. The TitleHorzAlign specification takes precedence, as shown in the following table.

| FlexItem.TitleBgColor | FlexView.TitleBgColor | Display color         |
|-----------------------|-----------------------|-----------------------|
| Unspecified           | Unspecified           | Default color         |
| Unspecified           | Specified             | FlexView.TitleBgColor |
| Specified             | unspecified           | FlexItem.TitleBgColor |
| Specified             | Specified             | FlexItem.TitleBgColor |


TitleHorzAlign example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>