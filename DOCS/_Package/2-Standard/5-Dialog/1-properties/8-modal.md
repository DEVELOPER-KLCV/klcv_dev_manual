---
layout: default

grand_parent: Dialog Class
parent: Properties
has_children: false
title: Dialog.Modal property
nav_order: 8
permalink: /package/standard/dialog/properties/modal
---
# {{ page.title }}


Specifies whether to display the dialog modally.

 

If $ TRUE , the dialog will be modal and you will not be able to move the parent hierarchy window.

 

The initial value is $ FALSE .

 

 

***Notes on internal execution of Internet Explorer***<br>
When running inside Internet Explorer (hereinafter referred to as IE) , modal control with a Dialog parent-child relationship of 3 levels or more does not work properly due to the balance between IE and Biz / Browser window control.

If you want to use Dialog modal control during IE internal execution , keep the hierarchy below 3 levels or define Dialog as a sibling relationship.

<small>Added since Ver.5.0.4 <br> Not supported in Mobile, AI</small>