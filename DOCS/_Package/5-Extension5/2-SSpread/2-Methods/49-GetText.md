---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetText Method
nav_order: 49
permalink: /package/extension5/sspread/methods/gettext
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetText(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
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
    Col = 1;
    Row = 1;
    CellType = $CellTypeCurrency;
    
    SetText(1, 1, "123.45");
    var ret = GetText(1, 1);
    print(ret, ret.classname, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> property<br><a href="/package/extension5/sspread/methods/getfloat">GetFloat</a>, <a href="/package/extension5/sspread/methods/getinteger">GetInteger</a>, <a href="/package/extension5/sspread/methods/settext">SetText</a> methods</td>
  </tr>
</table>
