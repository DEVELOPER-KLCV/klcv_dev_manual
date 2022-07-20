---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellFromScreenCoord Method
nav_order: 33
permalink: /package/extension5/sspread/methods/getcellfromscreencoord
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the column and row numbers of the cells displayed at the specified screen coordinates (x, y), with the top left coordinate of the spreadsheet as the origin.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellFromScreenCoord(<b>x</b>, <b>y</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-rvyq{border-color:inherit;font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-rvyq">Col</td>
    <td class="tg-0pky">The column number of the cell displayed at the position of the screen ( x, y ) coordinates. -1 for gray areas .</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-rvyq">Row</td>
    <td class="tg-0pky">The row number of the cell displayed at the position of the screen ( x, y ) coordinates. -1 for gray areas .</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>x</b></td>
    <td>Screen x coordinate</td>
  </tr>
  <tr>
    <td><b>y</b></td>
    <td>Screen y coordinate</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
   var ret = GetCellFromScreenCoord(100, 100);
    print(ret.Col, ret.Row, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/getcellpos">GetCellPos</a> method</td>
  </tr>
</table>
