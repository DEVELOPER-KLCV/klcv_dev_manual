---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Load Method
nav_order: 14
permalink: /package/csvpackage/csvdocument/methods/load
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Load CSV data from Reader object.<br>Data before Load method is executed will be lost.<br><br>When reading CSV data from a WEB server or file,<a href="/package/csvpackage/csvdocument/methods/get">Get</a> method can be used, but the Load method has more flexibility in functions such as being able to select the line to be read.<br><br><small><span style="color:red">Added since Ver.4.2.0 starts from here --><br></span></small>If the <a href="/package/csvpackage/csvdocument/methods/constructor#about-csvdocument-which-internal-character-code-is-unicodepc-ver-mobile-ver">internal character code is Unicode CSV Document</a>, the character code of the input CSV file is Unicode.<br><small><span style="color:red"><--till here<br></span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Load( <b>reader [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>reader</b></td>
    <td>Reader object <a href="/base/readerwriter#reader-object">ReaderObject</a> from which to read (object that can use the ReadLine method)</td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td>Search condition that specifies the row to read<br>Specify in the following format:-<br><code><pre>column [mode] operator value
    </pre></code><br><br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">column</th>
    <th class="tg-0pky">Specify the search key column with a column number starting from 0</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">mode</td>
    <td class="tg-0pky">Specify "n" when comparing the search key as a numerical value (compared as a character string if omitted)</td>
  </tr>
  <tr>
    <td class="tg-0pky">operator</td>
    <td class="tg-0pky">Specify the following comparison operators:-<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Operator</th>
    <th class="tg-kg9c">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">==</td>
    <td class="tg-0lax">Equal to the value</td>
  </tr>
  <tr>
    <td class="tg-0lax">!=</td>
    <td class="tg-0lax">Not equal to the value</td>
  </tr>
  <tr>
    <td class="tg-0lax">&gt; </td>
    <td class="tg-0lax">Greater than the value</td>
  </tr>
  <tr>
    <td class="tg-0lax">&gt;=</td>
    <td class="tg-0lax">Equal and greater the value</td>
  </tr>
  <tr>
    <td class="tg-0lax">&lt; </td>
    <td class="tg-0lax">Less than the value</td>
  </tr>
  <tr>
    <td class="tg-0lax">&lt;=</td>
    <td class="tg-0lax">Equal and less than the value</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td class="tg-0pky">value</td>
    <td class="tg-0pky">Specify the value to be compared. <br>If comparing the same row of different column, specify the column index with [ ].</td>
  </tr>
</tbody>
</table><br>Example:-<br><pre>"0==A"      1st column matches A row.<br>"1n>100"    the 2nd column matches row that bigger than 100th row.<br>"2==[3]"    3rd and 4th column matches the same row.<br><br>For the Search condition, the Maximum can be specified same as the number of column, and if want to specify multiple condition, combine them with AND. </pre>
    </td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-8</td>
    <td>Valid read object is not specified</td>
  </tr>
  <tr>
    <td>CSV-9</td>
    <td>Does not support ReadLine() method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.get("/test/sample.csv");
    csvdoc.Load(res, "1n>100", "2==[3]");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/save">Save</a>, <a href="/package/csvpackage/csvdocument/methods/get">Get</a>, <a href="/package/csvpackage/csvdocument/methods/parse">Parse</a> methods</td>
  </tr>
</table>



