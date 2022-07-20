---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadTextFile Method
nav_order: 63
permalink: /package/extension5/sspread/methods/loadtextfile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Read a text file.<br><br> the data delimiter can be specified in the text file. The column delimiter is used to split the column. The row delimiter is used to split the row. The default value is the line feed code. The cell delimiter is a character that is considered to be added to the left and right of the cell data when the character specified as the delimiter is included in the data. The default value is double quotes ("). <br><br> The <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a> method can be used to load a simple tab-delimited file.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadTextFile(<b>URL or Reader</b>, <b>celldelim</b>, <b>coldelim</b>, <b>rowdelim</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>URL or Reader</b></td>
    <td>Tab-delimited file URL or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br> The file will be cached on local computer for faster loading from the next time onwards if URL is specified. The latest files can be acquired from the server by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>  
  <tr>
    <td><b>celldelim</b></td>
    <td>A string representing the cell delimiter</td>
  </tr>  
  <tr>
    <td><b>coldelim</b></td>
    <td>A string representing the column delimiter</td>
  </tr>  
  <tr>
    <td><b>rowdelim</b></td>
    <td>A string representing the row delimiter</td>
  </tr>  
  <tr>
    <td><b>flags</b></td>
    <td>Method to read the file<br> Specify a combination of the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$LoadTextFileNoHeaders</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Do not set the header value</td>
  </tr>
  <tr>
    <td class="tg-0lax">$LoadTextFileColHeaders</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Set the first line of the text file to the value of the column header</td>
  </tr>
  <tr>
    <td class="tg-0lax">$LoadTextFileRowHeaders</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Set the first column of the text file to the row header value</td>
  </tr>
  <tr>
    <td class="tg-0lax">$LoadTextFileClearDataOnly</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">Erases all existing data when reading a text file and keeps only the format setting</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the LoadTextFile method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var session = findHttpSession("http://example.com");
    var res = session.Get("textfile.txt");
    LoadTextFile(res, "", ",", "", $LoadTextFileNoHeaders);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetotextfile">ExportRangeToTextFile</a>, <a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a>, <a href="/package/extension5/sspread/methods/loadfromfile">LoadFromFile</a>, <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
