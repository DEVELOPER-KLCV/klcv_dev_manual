---
layout: default

grand_parent: FlexRecord Class
parent: Properties
has_children: false
title: FlexRecord.StripedOpacity Property
nav_order: 5
permalink: /package/extension4/flexview/flexrecord/properties/stripedopacity
---
# {{ page.title }}

Specifies the transparency of odd rows when striping rows, at a ratio of 0 to 100.

If 0 is specified, it will be opaque and will have the same color as even lines. If 100 is specified, it will be completely transparent and white.

For odd-numbered rows: White is transparent with BgColor in a ratio of Striped Opacity.

For even lines: BgColor.

Display example

BgColor = $CCFFFF<br>
StripedOpacity=80

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexrecordp3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>