---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveBlockToBuffer Method
nav_order: 72
permalink: /package/extension5/sspread/methods/saveblocktobuffer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Saves all cell information in the specified range in ByteArray in binary format. -1 or 0 cannot be specified as the cell range. <br><br> Binary data is in SSpread's own format. It can be loaded using the <a href="/package/extension5/sspread/methods/loadblockfrombuffer">LoadBlockFromBuffer</a> method. <br><br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var data = SaveBlockToBuffer(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">ByteArray object containing cell information</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of the upper left cell of the cell range to save</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the upper left cell of the cell range to save</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of the lower right cell of the cell range to save</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the lower right cell of the cell range to save</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of SaveBlockToBuffer is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SaveBlockToBuffer method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var data = Spread1.SaveBlockToBuffer(1, 1, 10, 10);
    Spread2.LoadBlockFromBuffer(11, 11, 20, 20, data);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/loadblockfrombuffer">LoadBlockFromBuffer</a> method</td>
  </tr>
</table>
