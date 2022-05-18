---
layout: default

grand_parent: Doc Class
parent: Properties
has_children: false
title: Doc.Preview property
nav_order: 5
permalink: /package/standard/doc/properties/preview
---
# {{ page.title }}

Specify the print destination.

| Constant  | Value | Description                                               |
|-----------|:-----:|-----------------------------------------------------------|
| $ PRINTER |   0   | Outputs to the printer specified by the <a href="/package/standard/doc/properties/printer">Printer</a> property. |
| $ FILE    |   1   | Output the document as an SVG file. It does not print.    |
| $ SCREEN  |   2   | Display the preview screen.                               |

When debugging with Biz / Desiger , the preview screen is always displayed regardless of the property specified.

 
