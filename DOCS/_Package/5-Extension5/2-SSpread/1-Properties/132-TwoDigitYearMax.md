---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TwoDigitYearMax Property
nav_order: 132
permalink: /package/extension5/sspread/properties/twodigityearmax
---
# {{ page.title }}

Sets the base year for converting a 2-digit year to 4 digits.

The initial value is 2059 (year).

The 2-digit year display can be set with the <a href="/package/extension5/sspread/properties/typedatacentury">TypeDataCentury</a> property of a date cell (<a href="/package/extension5/sspread/properties/celltype">CellType</a> property is $CellTypeDate).

***Example with 2059***

Efefctive range of the year = 60 (1960) to 59 (2059)

| 2 digits | Year |
|:--------:|:----:|
|    58    | 2058 |
|    59    | 2059 |
|    60    | 1960 |
|    61    | 1961 |
|    62    | 1962 |

In this example, if the user enters 62, it will be interpreted as 1962.

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typedatacentury">TypeDataCentury</a> properties