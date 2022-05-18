---
layout: default

grand_parent: Doc Class
parent: Properties
has_children: false
title: Doc.Printer property
nav_order: 6
permalink: /package/standard/doc/properties/printer
---
# {{ page.title }}



Specify the printer name of the output destination. This is valid only when $ PRINTER is specified for the <a href="/package/standard/displayobject/properties/preview">Preview</a> Preview property.


A list of printers that can be used by Biz / Browser can be obtained with the <a href="/method/system/getPrinterList">getPrinterList</a> function.

If no printer is set on the PC, or if a printer name that is not set on the PC is specified, the preview screen will be displayed.

If a blank character string ("") is specified in the Printer property, the printer is output to the default printer set in Biz / Browser. The default printer for Biz / Browser is set with the <a href="/method/system/setDefaultPrinter">setDefaultPrinter</a> function.

When debugging with Biz / Desiger, the preview screen is always displayed regardless of the property specified.