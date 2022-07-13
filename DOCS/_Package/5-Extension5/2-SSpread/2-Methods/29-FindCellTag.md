---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.FindCellTag Method
nav_order: 29
permalink: /package/extension5/sspread/methods/findcelltag
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Searches for the tag set in the CellTag property and returns the cell position where the tag is set. If not found , returns null.<br><br>It has the following restrictions:<br> - CellTag can be set individually for sheet, row, column, and cell, but FingCellTag targets only cells.<br> - CellTag can set the same character string for multiple cells, but only the last set cell will be searched. <br> - If CellTag of the same character string is set in multiple cells, it will not be possible to search by that tag no matter which cell is deleted.<br><small><span style="color:red">Added since Ver.5.0.3</span></small> </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var rec = FindCellTag(<b>tag</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects <br><style type="text/css">
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
.tg .tg-imtw{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:left;vertical-align:top}
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
    <td class="tg-imtw">Col</td>
    <td class="tg-j5n6">Column index</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-imtw">Row</td>
    <td class="tg-j5n6">Row number</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>tag</b></td>
    <td>Tag string to search</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var rec = Spread1.FindCellTag("Summary items");
    if (rec != null) {
    Spread1.Col = rec.Col;
    Spread1.Row = rec.Row;
    Spread1.Text = data;
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property</td>
  </tr>
</table>
