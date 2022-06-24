---
layout: default

grand_parent: FlexView Class
parent: Properties
has_children: false
title: FlexView.CursorLineOpacity Property
nav_order: 7
permalink: /package/extension4/flexview/flexview/properties/cursorlineopacity
---
# {{ page.title }}

Specifies the cursor transparency of the cursor line in a ratio of 0 to 100.

The color that is actually displayed is the color that is transparently calculated by CursorLineOpacity for the background color of CursorColor and FlexRow.

If 0 is specified, it becomes opaque and is displayed as CursorColor regardless of the background color.

If you specify 100, it will be completely transparent and the line cursor will not be displayed.

Display example when FlexRow.BgColor = $ CCFFFF, CursorColor = $ 0000FF

CursorLineOpacity = 100<br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexviewp3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

CursorLineOpacity = 80<br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexviewp3.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

CursorLineOpacity = 60<br>
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexviewp3.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>
