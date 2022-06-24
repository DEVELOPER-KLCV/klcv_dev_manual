---
layout: default

grand_parent: FlexView Class
parent: Properties
has_children: false
title: FlexView.TitleHeight Property
nav_order: 23
permalink: /package/extension4/flexview/flexview/properties/titleheight
---
# {{ page.title }}

Specify the height of the title part. The default value is 20.

Display example


TitleHeight = 40<br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexviewp7.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

TitleHeight = 60<br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexviewp7.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

If you are using a FlexRowSet or FlexColumnSet, you may see a multi-row title. The height of each title row is the height specified in the TitleHeight property divided equally by the number of title rows displayed in that column.