---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellPos Method
nav_order: 34
permalink: /package/extension5/sspread/methods/getcellpos
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the left edge position, top edge position, column width, and row height of the specified cell.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellPos(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Number object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-rvyq{border-color:inherit;font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
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
    <td class="tg-rvyq">X</td>
    <td class="tg-0pky">Distance from the left edge of the spreadsheet to the left edge of the cell</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-rvyq">Y</td>
    <td class="tg-0pky">Distance from the top of the spreadsheet to the top of the cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Width</td>
    <td class="tg-0lax">Cell column width</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Height</td>
    <td class="tg-0lax">Cell row height</td>
  </tr>
</tbody>
</table>
The Value property returns $TRUE if the cell is in the display area, $FALSE otherwise .</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>	Cell row number</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
   var ret = GetCellPos(1, 1);
    if (ret == $TRUE) {
        MessageBox(strf("X coordinate:%1 Y coordinate:%2", ret.X, ret.Y));
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/getcellfromscreencoord">GetCelFromScreenCoord</a> method</td>
  </tr>
</table>
