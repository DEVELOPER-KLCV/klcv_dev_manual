---
layout: default

parent: 2. Standard Package
has_children: true

title: Graph Class
nav_order: 13
permalink: /package/standard/graph

---

# {{ page.title }}

<a href="/img/Package/Standard-Graph.PNG" target="_blank">
<img src="/img/Package/Standard-Graph.PNG" alt="login image"></a>

This class displays various graphs from numerical information.

 

The Graph class works in cooperation with the GraphAxis class and GraphSeries class.

To set the data to be displayed in the graph, you need to place the GraphAxis and GraphSeries objects in the structure defined below the Graph object.

**Object Structure**

<a href="/img/Package/Standard-ObjectStructure.PNG" target="_blank">
<img src="/img/Package/Standard-ObjectStructure.PNG" alt="login image"></a>

**Screen Display Example**


GraphType = $ BAR


{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std16.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br>

GraphType = $ LINE

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std16.files/image003.gif" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

<br>

GraphType=$PIE

{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std16.files/image004.gif" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

<br>

**Printer output by Doc class**


It prints just like the screen. 

<br>

**Default properties and ValueType**
 

The default property is <a href="/package/standard/form/properties/value">Value</a>. ValueType can be String, Number, Fixed and Date.

<br>

**Restrictions when visual style is enabled**

◆ Visual style specification is invalid.

<br>

**Precautions when scaling** 

Nothing in particular.



