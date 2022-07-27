---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RestrictCols Property
nav_order: 86
permalink: /package/extension5/sspread/properties/restrictcols
---
# {{ page.title }}

Set whether to restrict input in one column.

Specify the following values. The initial value is $FALSE.

| Constant | Description                                                                                                                                |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------|
| $TRUE    | Cannot be entered unless a value is entered in the column to the left (If you want to make sure that data is entered one column at a time) |
| $FALSE   | Can be entered in any column                                                                                                               |

If you specify $TRUE, you will not be able to enter one column at a time, so you can be sure to enter the values one column at a time.
If you try to enter one column apart, you will hear a beep and the <a href="/package/extension5/sspread/events/editerror">EditError</a> event will occur.

Set the row input limit with the <a href="/package/extension5/sspread/properties/restrictrows">RestrictRows</a> property.

Related Items<br>
<a href="/package/extension5/sspread/properties/restrictrows">RestrictRows</a> property<br>
<a href="/package/extension5/sspread/events/editerror">EditError</a>
event