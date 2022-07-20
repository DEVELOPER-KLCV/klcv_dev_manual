---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetClientArea Method
nav_order: 36
permalink: /package/extension5/sspread/methods/getclientarea
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the width and height of the spreadsheet display area (excluding the scrollbars).</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetClientArea()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Type</th>
    <th class="tg-z50u">Name</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Width</td>
    <td class="tg-0lax">Client area width</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Height</td>
    <td class="tg-0lax">Client area height</td>
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
    <td colspan="2"><code><pre>
   var ret = GetClientArea();
    print(ret.Width, ret.Height, "\n");
    </pre></code></td>
  </tr>
</table>
