---
layout: default

grand_parent: FlexHeader Class
parent: Properties
has_children: false
title: FlexHeader.Numbered Property
nav_order: 5
permalink: /package/extension4/flexview/flexheader/properties/numbered
---
# {{ page.title }}

Select whether to display the Value property value in the cell or the row number.

For $FALSE, the Value value is formatted and displayed with the Format property.

For $TRUE, the value of the Value property is preserved but not displayed, with line numbers starting at 1. Displaying line numbers is not formatted with the Format property.

Display Example

Numbered = $FALSE
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexheaderp1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

Numbered = $TRUE
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexheaderp1.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>