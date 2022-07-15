---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetText Method
nav_order: 88
permalink: /package/extension5/sspread/methods/settext
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the text in the specified cell.<br><br> This is the same function as setting the value with the <a href="/package/extension5/sspread/properties/text">Text</a> property. Use the <a href="/package/extension5/sspread/methods/setfloat">SetFloat</a> and <a href="/package/extension5/sspread/methods/setinteger">SetInteger</a> methods to set the cell value as a number.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetText(<b>col</b>, <b>row</b>, <b>text</b>)</td>
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
    <td><b>text</b></td>
    <td>Text to set</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetText method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties<br><a href="/package/extension5/sspread/methods/gettext">GetText</a>, <a href="/package/extension5/sspread/methods/setfloat">SetFloat</a>, <a href="/package/extension5/sspread/methods/setinteger">SetInteger</a> methods</td>
  </tr>
</table>
