---
layout: default

grand_parent: CheckBox Class
parent: Properties
has_children: false
title: FontFace property
nav_order: 4
permalink: /package/standard/checkbox/properties/fontface
---
# {{ page.title }}

Specifies font decoration attributes.

Specify a combination of the following values.

|Constant|Value|Description |
|--------|-----|------------|
|$STD    | 0   |Standard    |
|$BOLD   | 1   |Bold        |
|$ITALIC | 2   |Italic      |
|$UNDER  | 4   |Underlined  |
|$FIXED  | 8   | Monospaced (fixed pitch) font |


**<small>There are limits in AI. Please refer to <a href="/bizBrowserV/2/2-5/">the features and restrictions of the Android version</a>.</small>**

$BOLD + $ITALIC is displayed in highlighted italics.
If $FIXED is not specified, it is a proportional font.
