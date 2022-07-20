---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadFromBuffer Method
nav_order: 60
permalink: /package/extension5/sspread/methods/loadfrombuffer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Imports the contents of a spreadsheet stored in ByteArray in binary format into the spreadsheet currently being editing.<br><br>Binary data is in SSpread's own format. It can be saved using the SaveToBuffer method.<br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadFromBuffer(<b>data</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ByteArray <b>data</b></td>
    <td>ByteArray object containing binary format data</td>
  </tr>  
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of LoadFromBuffer is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the LoadFromBuffer method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var data = Spread1.SaveToBuffer();
    Spread2.LoadFromBuffer(data);
    </pre></code></td> 
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/savetobuffer">SaveToBuffer</a> method</td>
  </tr>
</table>
