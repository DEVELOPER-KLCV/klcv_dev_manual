---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetCellBorder Method
nav_order: 80
permalink: /package/extension5/sspread/methods/setcellborder
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the color and linetype of the border around the cell.<br><br>First, specify the target ruled line part in the argument index. To set a border around the cell range, specify the cell range with the arguments col, row, col2, row2, and specify $CellBorderIndexOutline for the argument index. To set a ruled line in one cell, set the column number (same value) in the arguments col and col2, and the row number (same value) in row and row2. <br><br>Use the <a href="/package/extension5/sspread/methods/getcellborder">GetCellBorder</a>  method to get the color and line type of the cell border.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetCellBorder(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>index</b>, <b>color</b>, <b>style</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of first cell</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the first cell</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of last cell</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the last cell</td>
  </tr>
  <tr>
    <td><b>index</b></td>
    <td>Border part to be set<br>Specify a combination of the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$CellBorderIndexLeft</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Left border of cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderIndexRight</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Right border of cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderIndexTop</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">Cell top border</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderIndexBottom</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">Bottom border of cells</td>
  </tr>
  <tr>
    <td class="tg-0lax">$CellBorderIndexOutline</td>
    <td class="tg-baqh">16</td>
    <td class="tg-0lax">Outer frame of cell range</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td><b>color</b></td>
    <td>Border color<br> Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a></td>
  </tr>
  <tr>
    <td><b>style</b></td>
    <td>Line type<br> Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-k3us{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-uysk{background-color:#FFF;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-ke5f{background-color:#D9D9D9;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-agra{background-color:#FFF;color:#5C5962;text-align:center;vertical-align:top}
.tg .tg-lsj2{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-lsj2"><span style="font-weight:normal;background-color:#D9D9D9">Constant</span></th>
    <th class="tg-k3us"><span style="font-weight:normal;background-color:#D9D9D9">Value</span></th>
    <th class="tg-ke5f"><span style="font-weight:normal;background-color:#D9D9D9">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleDefault</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">0</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">No borders (display default grid)</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleSolid</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">1</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Solid line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleDash</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">2</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Dashed line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">3</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Dotted line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleDashDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">4</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Dash dotted line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleDashDotDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">5</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Dash double-dotted line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleBlank</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">6</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Erase ruled lines and grid lines</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleFineSolid</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">11</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Line with every other dot</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleFineDash</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">12</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Fine dashed line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleFineDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">13</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Fine dotted line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleFineDashDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">14</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Fine dash dotted line</span></td>
  </tr>
  <tr>
    <td class="tg-uysk"><span style="background-color:#FFF">$CellBorderStyleFineDashDotDot</span></td>
    <td class="tg-agra"><span style="background-color:#FFF">15</span></td>
    <td class="tg-uysk"><span style="background-color:#FFF">Fine dash double-dotted line</span></td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetCellBorder method

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetCellBorder(2, 2, 2, 2, $CellBorderIndexOutline, $RED, $CellBorderStyleSolid);
    SetCellBorder(2, 4, 3, 6, $CellBorderIndexOutline, $BLUE, $CellBorderStyleDot);
    SetCellBorder(4, 2, 4, 6, $CellBorderIndexRight + $CellBorderIndexTop, $GREEN, $CellBorderStyleFineSolid);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/getcellborder">GetCellBorder</a> method</td>
  </tr>
</table>
