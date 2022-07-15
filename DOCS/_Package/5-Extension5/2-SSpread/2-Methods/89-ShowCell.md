---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ShowCell Method
nav_order: 89
permalink: /package/extension5/sspread/methods/showcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Scrolls the spreadsheet so that the specified cell appears in the specified position.<br> Scrolls the spreadsheet so that the specified cell appears in the specified position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ShowCell(<b>col</b>, <b>row</b>, <b>position</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>Column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number</td>
  </tr>
  <tr>
    <td><b>position</b></td>
    <td>Cell position <br> Specify the following values. <br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-k3us{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-cjvl{background-color:#FFF;border-color:inherit;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-y0ib{background-color:#FFF;border-color:inherit;color:#5C5962;text-align:center;vertical-align:top}
.tg .tg-gpky{background-color:#D9D9D9;border-color:inherit;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-lsj2{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-lsj2">Constant</th>
    <th class="tg-k3us">Value</th>
    <th class="tg-gpky">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-cjvl">$PositionUpperLeft</td>
    <td class="tg-y0ib">0</td>
    <td class="tg-cjvl">Upper left</td>
  </tr>
  <tr>
    <td class="tg-cjvl">$PositionUpperCenter</td>
    <td class="tg-y0ib">1</td>
    <td class="tg-cjvl">Upper center</td>
  </tr>
  <tr>
    <td class="tg-cjvl">$PositionUpperRight</td>
    <td class="tg-y0ib">2</td>
    <td class="tg-cjvl">Upper right</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionCenterLeft</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">Center left</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionCenter</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">Center</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionCenterRight</td>
    <td class="tg-baqh">5</td>
    <td class="tg-0lax">Center right</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionBottomLeft</td>
    <td class="tg-baqh">6</td>
    <td class="tg-0lax">Bottom left</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionBottomCenter</td>
    <td class="tg-baqh">7</td>
    <td class="tg-0lax">Bottom center</td>
  </tr>
  <tr>
    <td class="tg-0lax">$PositionBottomRight</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">Bottom right</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>ShowCell argument is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ShowCell method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (!IsVisible(10, 10, $FALSE)) {
        ShowCell(10, 10, $PositionUpperLeft);
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/leftcol">LeftCol</a>, <a href="/package/extension5/sspread/properties/toprow">TopRow</a> properties<br><a href="/package/extension5/sspread/methods/getbottomrightcell">GetBottomRightCell</a>, <a href="/package/extension5/sspread/methods/setactivecell">SetActiveCell</a> methods<br><a href="/package/extension5/sspread/events/topleftchange">TopLeftChange</a> event</td>
  </tr>
</table>
