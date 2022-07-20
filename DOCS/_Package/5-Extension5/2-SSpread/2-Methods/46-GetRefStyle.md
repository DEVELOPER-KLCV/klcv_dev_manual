---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetRefStyle Method
nav_order: 46
permalink: /package/extension5/sspread/methods/getrefstyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the cell reference style of the formula currently in use.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetRefStyle()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Cell reference style<br>Returns the following values:<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
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
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$RefStyleDefault</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Default cell reference<br>See the absolute coordinates of a matrix of letters and numbers.<br>The coordinates of the current matrix can be specified with a wildcard ( # ).<br>( A1, B #, # 2 )</td>
  </tr>
  <tr>
    <td class="tg-0lax">$RefStyleA1</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">" A1 " style cell reference<br>See relative coordinates of a matrix of letters and numbers.<br>Absolute coordinates can be specified with a  wildcard ( $ )<br>( $ A $ 1, $ B, $ 2, $ B2, C $ 5, D4 )</td>
  </tr>
  <tr>
    <td class="tg-0lax">$RefStyleR1C1</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">R1C1 style cell reference<br>See matrix coordinates using R and row numbers, C and column numbers.<br>The relative position from the current cell can be referred by enclosing the numerical value with "[]" .<br>If no number is specified after R or C, it is considered as the current row and column.<br>( R1C1, RC2, R4C [3], R [2] C4, RC [-2] )</td>
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
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetRefStyle();
    var style = "";
    switch (ret) {
        case $RefStyleDefault:
            style = "Default";
            break;
        case $RefStyleA1:
            style = "A1";
            break;
        case $RefStyleR1C1:
            style = "R1C1";
            break;
    }
    MessageBox("The reference style is " + style + " style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/formula">Formula</a> property<br><a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a>, <a href="/package/extension5/sspread/methods/setrefstyle">SetRefStyle</a> methods</td>
  </tr>
</table>
