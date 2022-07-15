---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetOddEvenRowColor Method
nav_order: 84
permalink: /package/extension5/sspread/methods/setoddevenrowcolor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the background color and text color for the odd-numbered and even-numbered lines, respectively.<br><br> If you have set the BackColor or ForeColor properties on individual cells, columns, or rows, those settings take precedence. If you want to get the background color and text color set for odd and even rows, use the GetOddEvenRowColor method.</td>
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
    <td>Background color for odd rows</td>
  </tr>
  <tr>
    <td><b>foreodd</b></td>
    <td>Text color of odd-numbered rows</td>
  </tr>
  <tr>
    <td><b>backeven</b></td>
    <td>Even row background color</td>
  </tr>
  <tr>
    <td><b>foreeven</b></td>
    <td>Text color of even-numbered rows</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetOddEvenRowColor method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/forecolor">ForeColor</a> properties<br><a href="/package/extension5/sspread/methods/getoddevenrowcolor">GetOddEvenRowColor</a> method</td>
  </tr>
</table>
