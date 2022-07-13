---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetBottomRightCell Method
nav_order: 31
permalink: /package/extension5/sspread/methods/getbottomrightcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the column and row numbers of the right and bottom cells of the spreadsheet in the display area.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetBottomRightCell()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pf8i{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Type</th>
    <th class="tg-cqgq">Name</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Col</td>
    <td class="tg-j5n6">Column number of the rightmost cell in the display area</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Row</td>
    <td class="tg-j5n6">Row number of the cell at the bottom of the display area</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the GetBottomRightCell method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetBottomRightCell();
    print(ret.Col, ret.Row, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/leftcol">LeftCol</a>, <a href="/package/extension5/sspread/properties/toprow">TopRow</a> properties</td>
  </tr>
</table>
