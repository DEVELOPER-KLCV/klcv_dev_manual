---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadFromFile Method
nav_order: 61
permalink: /package/extension5/sspread/methods/loadfromfile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Imports the contents of a spreadsheet saved in binary format into the spreadsheet currently being edited.<br><br>Binary files are SSpread's own format. It can be saved using the <a href="/package/extension5/sspread/methods/savetofile">SaveToFile</a> method. To load a text file separated by characters such as tabs, use the <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a> and <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a> methods.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadFromFile(<b>URL or Reader</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or Reader</b></td>
    <td>Binary file URL or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br> If URL is specified, the file will be cached on local computer for faster loading from the next time onwards. The latest files can always be acquired from the server by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>  
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the LoadFromFile method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.OpenDialog("Open", "SSpread Save Data(*.*)=*.*", "", "");
    LoadFromFile(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a>, <a href="/package/extension5/sspread/methods/savetofile">SaveToFile</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
