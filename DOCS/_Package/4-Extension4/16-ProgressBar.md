---
layout: default

parent: 4. Extension4 Package
has_children: true

title: ProgressBar Class
nav_order: 16
permalink: /package/extension4/progressbar

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-ProgressBar.PNG" target="_blank">
<img src="/img/Package/Ext4-ProgressBar.PNG" alt="login image"></a>

A class that displays a progress bar. The progress bar is a bar that extends horizontally or vertically and is used to display work progress.

There are two methods, one is to place it on a Form object and display it on the screen, and the other is to pop it up in a separate window.

**Screen Display Example**

BarStyle = $BLOCK<br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_progressbar.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

BarStyle = $VBLOCK<br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_progressbar.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

BarStyle = $SMOOTH<br>
{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_progressbar.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

BarStyle = $VSMOOTH<br>
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_progressbar.files/image004.png" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>

**Progress bar pop-up display**<br>
With the <a href="/package/extension4/progressbar/methods/popup">Popup</a> method, the progress bar can be displayed in a separate window.

{% assign img5 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_progressbar.files/image005.png" %}

<a href="{{ img5 }}" target="_blank"> <img src="{{ img5 }}" alt="{{img5}}"></a>

The ProgressBar object for pop-up display is created by the <a href="/package/extension4/progressbar/methods/create">Create</a> method.

The display position and size of the window to be displayed in the pop-up are specified by the <a href="/package/standard/displayobject/properties/x">X</a>, <a href="/package/standard/displayobject/properties/y">Y</a>, <a href="/package/standard/displayobject/properties/width">Width</a>, <a href="/package/standard/displayobject/properties/height">Height</a> property, and <a href="/package/extension4/progressbar/properties/position">Position</a> property of the ProgressBar object.

The <a href="/package/extension4/progressbar/properties/title">Title</a>, <a href="/package/extension4/progressbar/properties/autoclose">AutoClose</a>, <a href="/package/extension4/progressbar/properties/position">Position</a>, <a href="/package/extension4/progressbar/properties/popupbgcolor">PopupBGColor</a>, <a href="/package/extension4/progressbar/properties/popupfgcolor">PopupFGColor</a>, <a href="/package/extension4/progressbar/properties/message">Message</a>, and <a href="/package/extension4/progressbar/properties/cancelcaption">CancelCaption</a> properties are pop-up-only properties that set the look and behavior of the pop-up window.

**Printer output by Doc class**<br>
Not subject to printing.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/progressbar/properties/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>

**Restrictions when visual style is enabled**<br>
◆ The BarColor and BgColor properties are disabled because they give priority to the theme display.

**Precautions when scaling**<br>
Nothing in particular