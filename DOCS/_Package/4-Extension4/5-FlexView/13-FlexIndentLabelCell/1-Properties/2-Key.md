---
layout: default

grand_parent: FlexIndentLabelCell Class
parent: Properties
has_children: false
title: FlexIndentLabelCell.Key Property
nav_order: 2
permalink: /package/extension4/flexview/flexindentlabelcell/properties/key
---
# {{ page.title }}

This is the key value for displaying the indent.

The Key property is used together with the ParentKey property. Subsequent lines that have the same value in the ParentKey property as the value specified in the Key property will be connected and displayed as a parent and child.
Table example

| Row | Key Property Value | The value of the ParentKey property |
|:---:|:--------------------:|:-------------------------------------:|
|  1  | Kanto              |                                     |
|  2  | Tokyo              | Kanto                               |
|  3  | Ikebukuro          | Tokyo                               |
|  4  | Shinjuku           | Tokyo                               |
|  5  | Ueno               | Tokyo                               |
|  6  | Shinagawa          | Tokyo                               |
|  7  | Chiba              | Kanto                               |
|  8  | Funabashi          | Chiba                               |
|  9  | Narita             | Chiba                               |

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexilabelp1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>