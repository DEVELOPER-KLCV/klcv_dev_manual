---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetOddEvenRowColor Method
nav_order: 84
permalink: /package/extension5/sspread/methods/SetOddEvenRowColor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetOddEvenRowColor(<b>backodd</b>, <b>foreodd</b>, <b>backeven</b>, <b>foreeven</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>backodd</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>foreodd</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>backeven</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>foreeven</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td></td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/forecolor">ForeColor</a> properties<br><a href="/package/extension5/sspread/methods/GetOddEvenRowColor">GetOddEvenRowColor</a> method</td>
  </tr>
</table>
