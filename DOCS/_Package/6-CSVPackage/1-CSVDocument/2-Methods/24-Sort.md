---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Sort Method
nav_order: 24
permalink: /package/csvpackage/csvdocument/methods/sort
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sort CSV data.<br><br>The sort order can be arbitrarily specified by character string for key specification.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Sort( <b>key1 [, key2 [, key3, … ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>key</b></td>
    <td>Key specification string that specifies the sort order<br><br>Can specify at least one and as many as the number of columns at the maximum, and if want to  specify more than one, the specified order will be prioritized.<br><br>Specify in the following format:-<br><br><code><pre>
    column [mode] [arrangement]
    </pre></code><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">column</th>
    <th class="tg-0pky">Specify the column that will be the sort key with a column number starting from 0</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">mode mode</td>
    <td class="tg-0pky">Specify "n" when comparing the sort key as a numerical value (if omitted, comparison will be conducted  in character string)</td>
  </tr>
  <tr>
    <td class="tg-0lax">arrangement</td>
    <td class="tg-0lax">Specify "d" to sort in descending order (order in ascending if omitted)</td>
  </tr>
</tbody>
</table><br>Example:-<br>"0d"    First column in descending order by string comparison<br>"3nd"    4th column in descending order by numerical comparison<br>"1"    Second column in ascending order by string comparison</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc << Form1.Spread1.row;
    csvdoc.Sort("0d", "3nd", "1");
    Form1.Spread1.row << csvdoc;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



