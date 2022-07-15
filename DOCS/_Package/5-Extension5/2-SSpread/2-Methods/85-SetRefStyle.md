---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetRefStyle Method
nav_order: 85
permalink: /package/extension5/sspread/methods/setrefstyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the cell reference style of the formula.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetRefStyle(<b>style</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>style</b></td>
    <td>Cell reference style<br>Specify the following values.<br> <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-k3us{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-cjvl{background-color:#FFF;border-color:inherit;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-y0ib{background-color:#FFF;border-color:inherit;color:#5C5962;text-align:center;vertical-align:top}
.tg .tg-gpky{background-color:#D9D9D9;border-color:inherit;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-lsj2{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
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
    <td class="tg-cjvl">$RefStyleDefault</td>
    <td class="tg-y0ib">0</td>
    <td class="tg-cjvl">Default cell reference<br>See the absolute coordinates of a matrix of letters and numbers.<br>You can specify the coordinates of the current matrix with a wild card ( # ).<br>( A1, B #, # 2 )</td>
  </tr>
  <tr>
    <td class="tg-cjvl">$RefStyleA1</td>
    <td class="tg-y0ib">1</td>
    <td class="tg-cjvl">" A1 " style cell reference<br>See relative coordinates of a matrix of letters and numbers.<br>Absolute coordinates can be specified by wildcard ( $ )<br>( $ A $ 1, $ B, $ 2, $ B2, C $ 5, D4 )</td>
  </tr>
  <tr>
    <td class="tg-cjvl">$RefStyleR1C1</td>
    <td class="tg-y0ib">2</td>
    <td class="tg-cjvl">R1C1 style cell reference<br>See matrix coordinates using R and row numbers, C and column numbers.<br>You can refer to the relative position from the current cell by enclosing the numerical value with "[]" .<br>If you do not specify a number after R or C , it is considered as the current row and column.<br>( R1C1, RC2, R4C [3], R [2] C4, RC [-2] )</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-1</td>
    <td>The argument of SetRefStyle is invalid.

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Col = 1;
    Row = 1;
    SetRefStyle($RefStyleDefault);
    Formula = "B#";
    SetRefStyle($RefStyleA1);
    Formula = "$B1";
    SetRefStyle($RefStyleR1C1);
    Formula = "RC2";
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/formula">Formula</a> property<br><a href="/package/extension5/sspread/methods/getrefstyle">GetRefStyle</a>, <a href="/package/extension5/sspread/methods/recalccell">GetRefStyleReCalcCell</a> methods</td>
  </tr>
</table>
