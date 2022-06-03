---
layout: default

parent: 2. Standard Package
has_children: true

title: PulldownList Class
nav_order: 22
permalink: /package/standard/pulldownlist

---


# {{ page.title }}
<br>

<a href="/img/Package/Standard-PulldownList.PNG" target="_blank">
<img src="/img/Package/Standard-PulldownList.PNG" alt="login image"></a>

This class displays the pull-down list.

 

The PulldownList class works in tandem with the <a href="/package/standard/pulldownitem">PulldownItem</a> class.

To set the data to be displayed as choices, the PulldownItem class or its derived class objects must be placed in the structure defined below the PulldownList object.

**Object Structure**

<a href="/img/Package/PulldownList.gif" target="_blank">
<img src="/img/Package/PulldownList.gif" alt="login image"></a>


**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std11.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br><small><span style="color:green">In AI, selection candidates are displayed in full screen. Also, the Height property and <a href="/package/standard/pulldownlist/properties/dropdownwidth">DropdownWidth</a> property are ignored.</span></small>

<br>

**Printer Output by Doc class**

Not subject to printing.

<br>

**Default properties and ValueType**

The default property is <a href="/package/standard/pulldownlist/properties/value">Value</a> . The ValueType specification is invalid.

<br>

**Restrictions when visual style is enabled**

◆ BgColor is disabled on Windows Vista and later OS due to OS restrictions.

<br>

**Precautions when scaling**

◆ The apparent height (height not pulled down) is not affected by Vertical Scale, but is affected by the font size change by Font Scale.

◆ The width of the pull-down button is specified by the OS and is not subject to scaling.











