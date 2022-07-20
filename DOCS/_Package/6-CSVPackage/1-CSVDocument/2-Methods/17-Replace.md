---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Replace Method
nav_order: 17
permalink: /package/csvpackage/csvdocument/methods/replace
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Replace data in cells of specified column at once.<br>By stating the condition, selected cell can be replaced.<br><br><small><span style="color:red">Added since Ver.4.1.0 Mobile Ver.3.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = csvdoc.Replace( <b>row, col, val [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Number of updated cell.</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>row</b></td>
    <td>Column number starting with 0 on the column that starts the replacement.<br>The rows after the row specified by row will be replaced.</td>
  </tr>
  <tr>
    <td>integer <b>col</b></td>
    <td>Column number starts with 0 on the column that starts the replacement.</td>
  </tr>
  <tr>
    <td>String <b>val</b></td>
    <td>Character string to bet set.<br>The string can be specified directly, or can specify the value in another column in the following format.<br><code><pre>
    "[列番号]"
    </pre></code><br>Example:-<code><pre>
    "[3]"
    </pre></code><br>In this example,the cell that matches the condition is replaced with the values in the 4th column of the same row.<br><br>If the replacement string starts with "[", escape it with "\ [". Note that \ is an escape character in the CRS language, so if specify it as a string constant in a CRS script, \ must be specified twice.<br>Example:-<code><pre>
    "\\[12\\]"
    </pre></code></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td>Search criteria for cells to replace<br>Format is specified same as <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method.<br>Can specify as many search conditions as desired,as long as the maximum same as the number of columns, and if specify more than one, combine them with AND.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-14</td>
    <td>Incorrect column index</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Get("http://server/data1.csv");
    
    /* Updated the first column of every row to "new data" */
    csvdoc.Replace(0, 0, "new data");
    
    /* Update the second column of all rows to the same value as the third column */
    csvdoc.Replace(0, 1, "[2]");
    
    /* Updated the 5th column of the row where the 4th column is "1" to the same value as the 3rd column */
    csvdoc.Replace(0, 4, "[2]", "3==1");
    
    /* 6th column is the same row as 7th column, 8th column is updated to the same value as 3rd column */
    csvdoc.Replace(0, 7, "[2]", "5==[6]");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a>, <a href="/package/csvpackage/csvdocument/methods/find">Find</a> methods</td>
  </tr>
</table>



