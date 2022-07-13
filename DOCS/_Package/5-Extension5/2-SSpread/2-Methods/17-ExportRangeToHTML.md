---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportRangeToHTML Method
nav_order: 17
permalink: /package/extension5/sspread/methods/exportrangetohtml
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export a specific cell range to an HTML file. <br><br>A cell range specification has been added to the functionality of the <a href="/package/extension5/sspread/methods/exporttohtml">ExportToHTML</a> method. The cell range specified by the argument is exported regardless of the presence or absence of data in the cell.<br><br> Use the <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a> method to specify style information.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportRangeToHTML(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>Writer</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>col</b></td>
    <td>Start column number of cell range to export</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Start row number of cell range to export</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Last column number of cell range to export</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Last row number of cell range to export</td>
  </tr>
  
  <tr>
    <td><b>Writer</b></td>
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ExportRangeToHTML method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "HTMLFile(*.html)=*.html", "html", "");
    ExportRangeToHTML(1, 1, 10, 10, f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a>, <a href="/package/extension5/sspread/methods/exporttohtml">ExportToHTML</a>, <a href="/package/extension5/sspread/methods/exporttohtmlex">ExportToHTMLEx</a> methods</td>
  </tr>
</table>
