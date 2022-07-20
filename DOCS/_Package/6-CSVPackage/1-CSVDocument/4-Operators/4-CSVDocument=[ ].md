---
layout: default

grand_parent: CSVDocument Class
parent: Operators
has_children: false
title: CSVDocument << [ ] Operator
nav_order: 4
permalink: /package/csvpackage/csvdocument/operators/4
---
# {{ page.title }}

Loads the data of the array object on the right side of the CSVDocument object on the left side.

The array object that can be specified on the right side must have the following structure.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Type</th>
    <th class="tg-xt05">Example</th>
    <th class="tg-xt05">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">One -dimensional array<br> </td>
    <td class="tg-0lax"><code><pre>
    String data [];
    </pre></code></td>
    <td class="tg-0lax">The number of elements in the array corresponds to the number of rows in the CSV data.<br>The number of columns is one, and data itself corresponds to a column.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Two -dimensional equivalent array</td>
    <td class="tg-0lax"><code><pre>
    Record rec[] {
    String data1;
    String data2;
    }
    </pre></code></td>
    <td class="tg-0lax">The number of elements in the array corresponds to the number of rows in the CSV data.<br>The number of columns is the number of child objects, and data1 and data2 correspond to the columns.<br> </td>
  </tr>
</tbody>
</table>