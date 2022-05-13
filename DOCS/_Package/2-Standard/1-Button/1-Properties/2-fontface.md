---
layout: default

grand_parent: Button Class
parent: Properties
has_children: false
title: FontFace property
nav_order: 2
permalink: /package/standard/button/properties/fontface
---
# {{ page.title }}

Specifies font decoration attributes.

Specify a combination of the following values.

| Constant | Value | Description |
|----------|-------|-------------|
|$STD      | 0     | Standard    |
|$BOLD     | 1     | Bold        |
|$ITALIC   | 2     | Italic      |
|$UNDER    | 4     | Underlined      |
|$FIXED    | 8     | Monospaced (fixed pitch) font      |


**<small>There are limits to AI. Please refer to the <a href="/bizBrowserV/2/2-5/">features and restrictions of the Android version</a>.</small>**

$BOLD + $ITALIC is displayed in highlighted italics.
If $FIXED is not specified, it is a proportional font.