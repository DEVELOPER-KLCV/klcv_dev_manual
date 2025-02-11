---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetInteger Method
nav_order: 83
permalink: /package/extension5/sspread/methods/setinteger
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set integer values in numeric, currency, and percentage cells.<br><br> The Clip, ClipValue, Text, and Value for each properties can set the cell value as a string, but this method sets an integer value directly in the cell if the cell type is numeric, currency, or percentage.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetInteger(<b>col</b>, <b>row</b>, <b>value</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Cell row number</td>
  </tr>
  <tr>
    <td><b>value</b></td>
    <td>Integer value to set</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetInteger method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties<br><a href="/package/extension5/sspread/methods/getinteger">GetInteger</a>, <a href="/package/extension5/sspread/methods/setfloat">SetFloat</a>, <a href="/package/extension5/sspread/methods/settext">SetText</a> methods</td>
  </tr>
</table>
