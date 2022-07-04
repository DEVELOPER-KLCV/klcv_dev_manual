---
layout: default

grand_parent: ProgressBar Class
parent: Properties
has_children: false
title: ProgressBar.AutoClose Property
nav_order: 1
permalink: /package/extension4/progressbar/properties/autoclose
---
# {{ page.title }}

Set whether to automatically close the window popped up by the <a href="/package/extension4/progressbar/methods/popup">Popup</a> method.

If $TRUE is specified, the pop-up window is automatically closed when the step reaches the maximum value specified by the <a href="/package/extension4/progressbar/properties/step">Step</a> property.

If $FALSE is specified, the <a href="/package/extension4/progressbar/methods/popupclose">PopupClose</a> method will be called when the window is closed.