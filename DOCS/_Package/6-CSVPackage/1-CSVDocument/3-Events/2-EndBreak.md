---
layout: default

grand_parent: CSVDocument Class
parent: Events
has_children: false
title: CSVDocument.EndBreak Event
nav_order: 2
permalink: /package/csvpackage/csvdocument/events/endbreak
---
# {{ page.title }}

When loading CSV data into the array object to be printed, if a positive value is specified for the BreakKey property (<a href="/package/standard/spreadcolumn/properties/breakkey">SpreadColumn.BreakKey</a> property.etc) of the object corresponding to the column, after the data setting for the of the last row is completed, the EndBreak event will occur.The EndBreak event does not occur in a class that does not have a BreakKey property or a class that is not printed.

If positive value is specified in BreakKey property by the object in multiple columns, the EndBreak event will occur only at big object that has the highest absolute value.Also, if the value of the BreakKey property is the same, the EndBreak event will only occur for the previously defined object.
<br><br><small><span style="color:blue">Not supported in Mobile</span></small>