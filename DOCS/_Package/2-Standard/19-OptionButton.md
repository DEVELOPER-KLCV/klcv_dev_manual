---
layout: default

parent: 2. Standard Package
has_children: true

title: OptionButton Class
nav_order: 19
permalink: /package/standard/optionbutton

---

# {{ page.title }}

<br>

<a href="/img/Package/Standard-OptionButton.PNG" target="_blank">
<img src="/img/Package/Standard-OptionButton.PNG" alt="login image"></a>


A class that displays an option button to select one from multiple choices.

The OptionButton class works in tandem with the OptionItem class.

To set the data to be displayed as a choice, you need to place an object of the <a href="/package/standard/optionitem">OptionItem</a> class or its derived class in the structure defined under the OptionButton object.

**Object Structure**

<a href="/img/Package/OptionButton Object.gif" target="_blank">
<img src="/img/Package/OptionButton Object.gif" alt="login image"></a>

<br>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std5.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br>

**Printer Output by Doc class**

◎ indicating the selected status or ○ indicating the non-selected status is printed on the left side of the character string.

<br>

**Default properties and ValueType**

The default property is <a href="/package/standard/optionitem/properties/value">Value</a> . The ValueType specification is invalid.

<br>

**Restrictions when visual style is enabled**


◆ The FgColor property is disabled and follows the OS theme

<br>

**Precautions when scaling**
 

Nothing in particular






