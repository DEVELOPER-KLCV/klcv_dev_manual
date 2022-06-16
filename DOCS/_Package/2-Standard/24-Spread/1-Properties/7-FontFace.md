---
layout: default

grand_parent: Spread Class
parent: Properties
has_children: false
title: FontFace Property
nav_order: 7
permalink: /package/standard/spread/properties/fontface
---
# {{ page.title }}
<br>

Specifies font decoration attributes.

Specify the combination of the following values.

| Constant | Value |          Description          |
|:--------:|:-----:|:-----------------------------:|
|   $ STD  |   0   |            Standard           |
|  $ BOLD  |   1   |              Bold             |
| $ ITALIC |   2   |            Italics            |
|  $ UNDER |   4   |           Underline           |
|  $ FIXED |   8   | Monospaced (fixed pitch) font |


<small><span style="color:blue"><br><small>There are limits for AI. Please refer to the <a href="/bizBrowserV/2/2-5/">Android Version Features and Restrictions</a>.</small></span></small>


$ BOLD + $ ITALIC is displayed in highlighted italics.

If $ FIXED is not specified, it is a proportional font.
