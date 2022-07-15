---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellBorder Method
nav_order: 32
permalink: /package/extension5/sspread/methods/getcellborder
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the color and line type of the border around the cell. <br>Use the <a href="/package/extension5/sspread/methods/setcellborder">SetCellBorder</a> method to set the cell border.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellBorder(<b>col</b>, <b>row</b>, <b>index</b>)</td>
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
    <td class="tg-j5n6">Number<br>UString</td>
    <td class="tg-pf8i">Color</td>
    <td class="tg-j5n6">Border color<br>Able to get the <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a></td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Style </td>
    <td class="tg-j5n6">Line type<br>Returns the following values:<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-23hc">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$CellBorderStyleDefault</td>
    <td class="tg-j5n6">0</td>
    <td class="tg-j5n6">No borders (display default grid)</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$CellBorderStyleSolid</td>
    <td class="tg-j5n6">1</td>
    <td class="tg-j5n6">Solid line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleDash</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">Dashed line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleDot</td>
    <td class="tg-0lax">3</td>
    <td class="tg-0lax">Dotted line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleDashDot</td>
    <td class="tg-0lax">4</td>
    <td class="tg-0lax">Dash dotted line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleDashDotDot</td>
    <td class="tg-0lax">5</td>
    <td class="tg-0lax">Dash double-dotted line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleBlank</td>
    <td class="tg-0lax">6</td>
    <td class="tg-0lax">Erase ruled lines and grid lines</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleFineSolid</td>
    <td class="tg-0lax">11</td>
    <td class="tg-0lax">Line with every other dot</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleFineDash</td>
    <td class="tg-0lax">12</td>
    <td class="tg-0lax">Fine dashed line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleFineDot</td>
    <td class="tg-0lax">13</td>
    <td class="tg-0lax">Fine dotted line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleFineDashDot</td>
    <td class="tg-0lax">14</td>
    <td class="tg-0lax">Fine dash dotted line</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderStyleFineDashDotDot</td>
    <td class="tg-0lax">15</td>
    <td class="tg-0lax">Fine dash double-dotted line</td>
  </tr>
</tbody>
</table></td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Cell row number</td>
  </tr>
  <tr>
    <td><b>index</b></td>
    <td>Ruled line part to be acquired<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
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
    <td class="tg-0pky">$CellBorderIndexLeft</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Left border of cell</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ CellBorderIndexRight</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Right border of cell</td>
  </tr>
  <tr>
    <td class="tg-0pky">$CellBorderIndexTop</td>
    <td class="tg-c3ow">4</td>
    <td class="tg-0pky">Cell top border</td>
  </tr>
  <tr>
    <td class="tg-0pky">$CellBorderIndexBottom</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-0pky">Bottom border of cell</td>
  </tr>
  <tr>
    <td class="tg-0pky">$CellBorderIndexOutline</td>
    <td class="tg-c3ow">16</td>
    <td class="tg-0pky">Outer frame of cell range</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetCellBorder(1, 1, $CellBorderIndexLeft);
    var style = "";
    switch (ret.Style){
        case $CellBorderStyleDefault:
            style = "No ruled lines";
            break;
        case $CellBorderStyleSolid:
            style = "Solid line";
            break;
        default:
            style = "Others";
            break;
    }
    MessageBox("The ruled line on the left side of (1, 1)「" + style + "」で、colour is" + str(ret.Color));
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/setcellborder">SetCellBorder</a> method</td>
  </tr>
</table>
