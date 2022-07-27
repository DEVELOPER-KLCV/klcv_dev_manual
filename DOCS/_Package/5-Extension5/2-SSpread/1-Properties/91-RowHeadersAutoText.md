---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RowHeadersAutoText Property
nav_order: 91
permalink: /package/extension5/sspread/properties/rowheadersautotext
---
# {{ page.title }}

Sets whether to display letters or numbers in the line header or leave them blank.

Specify the following values. The initial value is $DispNumbers.

| Constant     | Value | Description             |
|--------------|:-----:|-------------------------|
| $DispBlank   |   0   | Blank                   |
| $DispNumbers |   1   | Display numbers |
| $DispLetters |   2   | Display letters      |

Column headers are set with the <a href="/package/extension5/sspread/properties/colheadersautotext">ColHeadersAutoText</a> property.

The characters (A, B, C and 1, 2, 3) displayed with $DispNumbers and $DispLetters are not set as cell values. When you refer to the cell value with the <a href="/package/extension5/sspread/properties/text">Text</a> property or <a href="/package/extension5/sspread/properties/value">Value</a> property, a blank string is returned. When you set a value in the header cell with the Text property or Value property, the display of that value has priority. If you set a blank character string, it will return to the original display.

Related Item<br>
<a href="/package/extension5/sspread/properties/colheadersautotext">ColHeadersAutoText</a> property