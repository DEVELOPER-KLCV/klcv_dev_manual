---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Form.Transparent property
nav_order: 10
permalink: /package/standard/form/properties/transparent
---
# {{ page.title }}

<br>

$ TRUE disables the <a href="/package/standard/form/properties/bgcolor">BgColor</a> property and makes the background transparent.

It does not work for root and Form directly under Dialog (the specification is ignored).


**Limitations**

This function is realized by interrupting the drawing mechanism of the OS. Therefore, there are the following restrictions regarding usage.

- Due to the drawing mechanism , transparent forms are redrawn more often than normal objects. Therefore , it is not suitable for dynamic representation ( such as moving in real time ) .

- If a transparent Form is placed on a Form that has child objects, the hierarchical relationship between the child objects on each Form may not be expressed correctly.

<br><small><span style="color:red">Added since Ver.5.0.4</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> 