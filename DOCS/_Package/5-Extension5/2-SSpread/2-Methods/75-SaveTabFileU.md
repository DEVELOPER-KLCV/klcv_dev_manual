---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveTabFileU Method
nav_order: 75
permalink: /package/extension5/sspread/methods/savetabfileu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Save the spreadsheet data in a Unicode tab-delimited file. <br><br>It has the same function as the SaveTabFile method, but the output result is a Unicode text file. <br><br>Use the ExportToTextFileU method to specify any delimiter.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SaveTabFileU(<b>Writer</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>Writer</b></td>
    <td>Save to <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SaveTabFileU method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Tab delimited file(*.txt)=*.txt", "", "");
    SaveTabFileU(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exporttotextfileu">ExportToTextFileU</a>, <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a>, <a href="/package/extension5/sspread/methods/savetabfile">SaveTabFile</a>, <a href="/package/extension5/sspread/methods/savetofile">SaveToFile</a> methods</td>
  </tr>
</table>
