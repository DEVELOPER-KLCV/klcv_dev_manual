---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetOddEvenRowColor Method
nav_order: 45
permalink: /package/extension5/sspread/methods/getoddevenrowcolor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the background color and text color set for odd-numbered and even-numbered lines.<br><br>Use the <a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a> method to set the background and text colors for odd and even rows.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetOddEvenRowColor()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
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
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Type</th>
    <th class="tg-z50u">Name</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number<br>UString</td>
    <td class="tg-ihln">BackOdd</td>
    <td class="tg-0lax">Background color for odd rows</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number<br>UString</td>
    <td class="tg-ihln">ForeOdd</td>
    <td class="tg-0lax">Character color of odd rows</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number<br>UString</td>
    <td class="tg-ihln">BackEven</td>
    <td class="tg-0lax">Even row background color</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number<br>UString</td>
    <td class="tg-ihln">ForeEven</td>
    <td class="tg-0lax">Even row text color</td>
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
    <td>An error occurred in the GetOddEvenRowColor method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetOddEvenRowColor($CCFFFF, $006666, $FFFFCC, $666600);
    var ret = GetOddEvenRowColor();
    print(ret.BackOdd, ret.ForeOdd, ret.BackEven, ret.ForeEven, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a> method</td>
  </tr>
</table>
