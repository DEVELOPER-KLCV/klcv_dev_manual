---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Form.BgPattern property
nav_order: 4
permalink: /package/standard/form/properties/bgpattern
---
# {{ page.title }}

<br><br>
Specify whether to cache the SVG to be displayed in the background as image data or to render the SVG each time it is drawn .

 

If $ TRUE is specified, it will be cached as image data. In this case, the initial display takes time and consumes memory for the cache, but once displayed, redrawing is very fast.

If $ FALSE is specified, the SVG will be rendered and displayed directly. In this case, memory consumption can be saved because no image data is created.

<br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>