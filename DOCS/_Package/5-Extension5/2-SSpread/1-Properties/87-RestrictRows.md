---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RestrictRows Property
nav_order: 87
permalink: /package/extension5/sspread/properties/restrictrows
---
# {{ page.title }}

Set whether to limit the input of one line apart.

Specify the following values. The initial value is $FALSE.

| Constant | Description                                                                                                                  |
|----------|------------------------------------------------------------------------------------------------------------------------------|
| $TRUE    | Cannot be entered unless a value is entered in the next row above (If you want to make sure that data is entered row by row) |
| $FALSE   | Can be entered on any row.                                                                                                   |

If you specify $ TRUE, you will not be able to enter one row at a time, so you can be sure to enter the value row by row.
If you try to enter one row apart, you will hear a beep and the <a href="/package/extension5/sspread/events/editerror">EditError</a> event will occur.

  Set the column input limit with the <a href="/package/extension5/sspread/properties/restrictcols">RestrictCols</a> property.

  Related Items<br>
<a href="/package/extension5/sspread/properties/restrictcols">RestrictCols</a> property<br>
<a href="/package/extension5/sspread/events/editerror">EditError</a>
event