---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.TitleVertAlign Property
nav_order: 8
permalink: /package/extension4/flexview/flexitem/properties/titlevertalign
---
# {{ page.title }}

Specifies the vertical assignment of column titles.

In addition to the TitleVertAlign property, the title assignment is also affected by the VerticalAlign property defined by FlexLabel, FlexTextBox, and so on. The TitleVertAlign specification takes precedence, as shown in the following table.

| TitleVertAlign | VerticalAlign | Layout                  |
|----------------|---------------|-------------------------|
| Unspecified    | Unspecified   | Centered                |
| Unspecified    | Specified     | Follow Vertical Align   |
| Specified      | Unspecified   | Follow Title Vert Align |
| Specified      | Specified     | Follow Title Vert Align |

TitleVertAlign example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp4.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<small><span style="color:red">Added since Ver.4.1.0</span></small>