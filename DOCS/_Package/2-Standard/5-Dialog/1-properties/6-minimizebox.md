---
layout: default

grand_parent: Dialog Class
parent: Properties
has_children: false
title: Dialog.MinimizeBox property
nav_order: 6
permalink: /package/standard/dialog/properties/minimizebox
---
# {{ page.title }}

Specifies whether to enable / disable the "Minimize" button in the dialog.

 

If you specify $ TRUE , the "Minimize" button will be displayed and enabled, and you can minimize it by user operation.

 

The initial value is $ FALSE .

 

If $ FALSE is specified with the Dialog.MaximizeBox property , the button will be hidden.

If the Dialog.MaximizeBox property is specified for $ TRUE and $ FALSE is specified for the MinimizeBox property , the Minimize button will be disabled.

<small>Added since Ver.4.1.0 <br> Not supported in Mobile, AI</small>