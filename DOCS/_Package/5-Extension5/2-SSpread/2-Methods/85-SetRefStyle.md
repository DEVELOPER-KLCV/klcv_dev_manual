---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetRefStyle Method
nav_order: 85
permalink: /package/extension5/sspread/methods/SetRefStyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
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
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-1</td>
    <td></td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/formula">Formula</a> property<br><a href="/package/extension5/sspread/methods/GetRefStyle">GetRefStyle</a>, <a href="/package/extension5/sspread/methods/ReCalcCell">GetRefStyleReCalcCell</a> methods</td>
  </tr>
</table>
