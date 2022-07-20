---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetFloat Method
nav_order: 41
permalink: /package/extension5/sspread/methods/getfloat
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets floating point values from numeric, currency, and percentage cells.<br><br>The <a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a> and <a href="/package/extension5/sspread/properties/value">Value</a> properties can be referred directly to the cell's value as a string, but this method takes the floating point value in the cell if the cell type is numeric, currency, or percent.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetFloat(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Floating point value</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>col</td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td>row</td>
    <td>Cell row number</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the GetFloat method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties<br><a href="/package/extension5/sspread/methods/getinteger">GetInteger</a>, <a href="/package/extension5/sspread/methods/gettext">GetText</a>, <a href="/package/extension5/sspread/methods/setfloat">SetFloat</a> method</td>
  </tr>
</table>
