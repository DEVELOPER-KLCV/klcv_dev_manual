---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColHeadersAutoText Property
nav_order: 33
permalink: /package/extension5/sspread/properties/colheadersautotext
---
# {{ page.title }}

Sets whether to display characters or numbers in the column headers or leave them blank.

Specify the following values. The initial value is $DispLetters.

| Constant     | Value | Description        |
|--------------|:-----:|--------------------|
| $DispBlank   |   0   | Blank              |
| $DispNumbers |   1   | Display numbers    |
| $DispLetters |   2   | Display characters |

Row headers are set in the <a href="/package/extension5/sspread/properties/rowheadersautotext">RowHeadersAutoText</a> property.

The characters (A, B, C and 1, 2, 3) displayed with $ DispNumbers and $ DispLetters are not set as cell values. Referencing a cell value with the <a href="/package/extension5/sspread/properties/text">Text</a> or <a href="/package/extension5/sspread/properties/value">Value</a> properties will return a blank string. When set a value in the header cell with the Text property or Value property, the display of that value has priority. If set a blank character string, it will return to the original display.

Related Item<br>
<a href="/package/extension5/sspread/properties/rowheadersautotext">RowHeadersAutoText</a> property