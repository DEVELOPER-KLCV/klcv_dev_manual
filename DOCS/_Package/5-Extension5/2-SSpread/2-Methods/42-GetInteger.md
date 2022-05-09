---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetInteger Method
nav_order: 42
permalink: /package/extension5/sspread/methods/GetInteger
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetInteger(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>col</td>
    <td></td>
  </tr>
  <tr>
    <td>row</td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Col = 1;
    Row = 1;
    CellType = $CellTypeCurrency;
    
    SetInteger(1, 1, 12345);
    var ret = GetInteger(1, 1);
    print(ret, ret.classname, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/Clip">Clip</a>, <a href="/package/extension5/sspread/properties/ClipValue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/Value">Value</a> properties<br><a href="/package/extension5/sspread/methods/GetFloat">GetFloat</a>, <a href="/package/extension5/sspread/methods/GetText">GetText</a>, <a href="/package/extension5/sspread/methods/SetInteger">SetInteger</a> method</td>
  </tr>
</table>
