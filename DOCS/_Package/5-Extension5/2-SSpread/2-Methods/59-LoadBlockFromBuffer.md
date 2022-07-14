---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadBlockFromBuffer Method
nav_order: 59
permalink: /package/extension5/sspread/methods/loadblockfrombuffer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Imports the contents of a spreadsheet stored in ByteArray in binary format into the spreadsheet currently being editing.-1 or 0 cannot be specified as the cell range.Even if it is specify a range larger than the range saved by SaveBlockToBuffer, it will be the range up to the range acquired by <a href="/package/extension5/sspread/methods/saveblocktobuffer">SaveBlockToBuffer</a>.<br><br>Binary data is in SSpread's own format. It can be saved using the SaveBlockToBuffer method.<br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadBlockFromBuffer(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>data</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of the upper left cell of the cell range to be read</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the upper left cell of the cell range to be read</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of the lower right cell of the cell range to be read</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the lower right cell of the cell range to be read</td>
  </tr>
  <tr>
    <td><b>data</b></td>
    <td>ByteArray object containing binary format data</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of LoadBlockFromBuffer is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the LoadBlockFromBuffer method</td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/saveblocktobuffer">SaveBlockToBuffer</a> method</td>
  </tr>
</table>
