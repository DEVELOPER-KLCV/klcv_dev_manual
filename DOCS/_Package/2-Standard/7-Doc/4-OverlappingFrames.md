---
layout: default

grand_parent: 2. Standard Package
parent: Doc Class

title: Printing overlapping frames
nav_order: 4
permalink: /package/standard/doc/print_overlap_frames

---



# {{ page.title }}

To print the arrayed objects with overlapping borders, set the <a href="/package/standard/displayobject/properties/layoutmargin">LayoutMargin</a> property to -2.

LayoutMargin = 0;

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


LayoutMargin = -2;

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-1.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>


Adjust the <a href="/package/standard/displayobject/properties/x">X</a> and <a href="/package/standard/displayobject/properties/y">Y</a> properties to overlay the borders of the form .

  

X = 0;
Y = 0;
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-1.files/image003.gif" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>


X = -2;
Y = -2;
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-1.files/image004.gif" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>
