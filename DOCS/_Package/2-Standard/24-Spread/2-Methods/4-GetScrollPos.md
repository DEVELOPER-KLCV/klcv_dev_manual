---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: Spread.GetScrollPos Method
nav_order: 4
permalink: /package/standard/spread/methods/getscrollpos
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the current scroll position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var pos = Spread1.GetScrollPos( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the scroll position (top row displayed) with the first row as 0.<br>Since Ver.3.1.2.0, the following child objects have been added to the return value.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-spl2{border-color:#000000;font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-npz6{background-color:#c0c0c0;border-color:#000000;text-align:center;vertical-align:top}
.tg .tg-wp8o{border-color:#000000;text-align:center;vertical-align:top}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-npz6">Type</th>
    <th class="tg-npz6">Name</th>
    <th class="tg-f7v4">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-wp8o">Number</td>
    <td class="tg-spl2">row</td>
    <td class="tg-73oq">Row position displayed on the top line<br>Same as the Value property of the return value.</td>
  </tr>
  <tr>
    <td class="tg-wp8o">Number</td>
    <td class="tg-spl2">col</td>
    <td class="tg-73oq">Column position displayed in the leftmost column<br>Returns the position of the column displayed in the leftmost column. The first column will be 0.</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre></pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/spread/methods/setscrollpos">SetScrollPos</a> method</td>
  </tr>
</table>



