---
layout: default

grand_parent: EditObject Class
parent: Properties
has_children: false
title: FontFace property
nav_order: 6
permalink: /package/standard/editobject/properties/fontface
---
# {{ page.title }}


Specifies font decoration attributes.

 

Specify a combination of the following values.

| Constant | Value | Description                   |
|----------|:-----:|-------------------------------|
| $ STD    |   0   | Standard                      |
| $ BOLD   |   1   | Bold                          |
| $ ITALIC |   2   | Italics                       |
| $ UNDER  |   4   | Underline                     |
| $ FIXED  |   8   | Monospaced (fixed pitch) font |

<br><small><span style="color:blue">There are limits to AI. Please refer to the [features and restrictions of the Android version]().</span></small>


$ BOLD + $ ITALIC is displayed in italics.

If $ FIXED is not specified, it is a proportional font.