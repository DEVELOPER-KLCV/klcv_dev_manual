---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetFloat Method
nav_order: 82
permalink: /package/extension5/sspread/methods/setfloat
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set floating point values for numeric, currency, and percentage cells.<br><br>The <a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a> and <a href="/package/extension5/sspread/properties/value">Value</a> for each properties can be set the cell value as a string, but this method sets the floating point value directly to the cell if the cell type is numeric, currency, or percentage.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetFloat(<b>col</b>, <b>row</b>, <b>value</b>)</td>
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
    <td>Floating point value to set</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetFloat method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Col = 1;
    Row = 1;
    CellType = $CellTypeCurrency;
    
    SetFloat(1, 1, 123.45);
    var ret = GetFloat(1, 1);
    print(ret, ret.classname, "\n");   
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties<br><a href="/package/extension5/sspread/methods/getfloat">GetFloat</a>, <a href="/package/extension5/sspread/methods/setinteger">SetInteger</a>, <a href="/package/extension5/sspread/methods/settext">SetText</a> methods</td>
  </tr>
</table>
