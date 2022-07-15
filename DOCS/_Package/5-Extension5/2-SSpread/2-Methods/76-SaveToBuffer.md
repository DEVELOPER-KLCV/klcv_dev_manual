---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveToBuffer Method
nav_order: 76
permalink: /package/extension5/sspread/methods/savetobuffer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Saves all the information in the spreadsheet in binary format in ByteArray.<br><br> Binary data is in SSpread's own format. It can be loaded using the <a href="/package/extension5/sspread/methods/loadfrombuffer">LoadFromBuffer</a> method. <br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var data = SaveToBuffer()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">ByteArray object that stores sheet information</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>Error in SaveToBuffer method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/loadfrombuffer">LoadFromBuffer</a> method</td>
  </tr>
</table>
