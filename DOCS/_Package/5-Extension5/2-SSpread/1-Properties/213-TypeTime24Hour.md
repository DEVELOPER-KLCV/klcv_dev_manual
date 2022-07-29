---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTime24Hour Property
nav_order: 213
permalink: /package/extension5/sspread/properties/typetime24hour
---
# {{ page.title }}


In the time cell, set the time display format.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeTime .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is the OS setting value.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Constant</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Example ( 23:00 )</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$TypeTime24Hour12HourClock</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">11:00 pm</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeTime24Hour24HourClock</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">23:00</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeTime12HourClockAm</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">11:00 pm</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeTime12AmHourClock</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">11:00 pm</td>
  </tr>
</tbody>
</table>

Set the <a href="/package/extension5/sspread/properties/typetimeseconds">TypeTimeSeconds</a> property to $TRUE to display "seconds" .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for time cells .

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeTime;
TypeTime24Hour = $TypeTime24Hour12HourClock;
Value = str(sysdate(), "HHMISS");
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeTime;
TypeTime24Hour = $TypeTime12AmHourClock;
Value = str(sysdate(), "HHMISS");
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typetimeseconds">TypeTimeSeconds</a> properties