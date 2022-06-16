---
layout: default

grand_parent: ComboBox Class
parent: Properties
has_children: false
title: ComboBox.AutoTab Property
nav_order: 1
permalink: /package/extension4/combobox/properties/autotab
---
# {{ page.title }}
<br>

If specify $TRUE, the focus automatically moves to the next object when the choice is confirmed by key input.

Only valid if the <a href="/package/extension4/combobox/properties/editable">Editable</a> property is $FALSE.

When the corresponding option is narrowed down to only one by key input, the value is confirmed as input and the focus moves.

Example

<ol>
<li>Initial state</li>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_combobp3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a><br><br>

<li>When you enter ‘2’, the beginning of the options starting with ‘2’ is displayed.</li>

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_combobp3.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a><br><br>

<li>When you enter 1', the only option that matches '21' is "21: Gifu", so it will be confirmed.</li>
   
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_combobp3.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a><br><br>

<li>Assuming that "21: Gifu" has been entered, the focus will be automatically moved to the next object.</li>
   
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_combobp3.files/image004.png" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>

</ol>