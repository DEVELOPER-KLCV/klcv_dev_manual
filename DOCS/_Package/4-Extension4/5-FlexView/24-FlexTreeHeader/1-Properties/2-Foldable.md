---
layout: default

grand_parent: FlexTreeHeader Class
parent: Properties
has_children: false
title: FlexTreeHeader.Foldable Property
nav_order: 2
permalink: /package/extension4/flexview/flextreeheader/properties/foldable
---
# {{ page.title }}

Specifies that the tree can be collapsed by screen operation.

If you specify $ TRUE, a collapse icon is displayed, and you can collapse or undo the tree with a left mouse click. You can also use the left arrow key to collapse the tree and the right arrow key to undo it.

If you specify $ FALSE, the collapse icon will not be displayed and you will not be able to collapse the tree by operating the screen.

The Foldable property cannot be specified individually for each row.

Display example


Foldable = $TRUE

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flextheaderp1.files/image002.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

---

Foldable = $FALSE

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flextheaderp1.files/image003.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>
