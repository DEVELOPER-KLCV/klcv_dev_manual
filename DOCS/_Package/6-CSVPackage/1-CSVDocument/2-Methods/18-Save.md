---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Save Method
nav_order: 18
permalink: /package/csvpackage/csvdocument/methods/save
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Save CSV data in Writer object.<br><br><small><span style="color:red">Added since Ver.4.2.0, From here--></span></small>If <a href="/package/csvpackage/csvdocument/methods/constructor#about-csvdocument-which-internal-character-code-is-unicodepc-ver-mobile-ver">the internal character code is Unicode CSV Document</a>, the character code of the saved CSV file will be Unicode.<br><small><span style="color:red">Till here<--</span></small><br><br><small><span style="color:green">Since AI Ver.1.0.1 and onwards, the internal character code will always be in UTF-8.</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Save( <b>writer [, cond1 [, cond2, … ] ]</b> )<br><br><small><span style="color:green">Since Version 5.0.3, the following formats are possible</span></small><br>csvdoc.Save( <b>writer [, delimiter [, cond1 [, cond2, … ] ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>Object <b>writer</b></td>
    <td><a href="/base/readerwriter#reader-object">WriterObject</a> to save to</td>
  </tr>
  <tr>
    <td>String <b>delimiter</b></td>
    <td>Change the delimeter character during the output from the default comma (,). <br>Can be spcified by using "d = [delimiter character]".Only one character can be specified for the delimiter.<br>For tab delimiter, specify it as "d = \ t".<br>If delimiter is changed, no quotes will be executed.<br><br>If the second argument is not considered as a delimiter specification, it is considered as a Search condition specification.<br><br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td>Search criteria that specify the rows to be saved<br><br>Specify in the same format as the <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method.<br>Can specify as many search conditions as desired, as long as the maximum are same as number of columns, and if more than one is specified, combine them with AND.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-11</td>
    <td>Valid Write object is not specified</td>
  </tr>
  <tr>
    <td>CSV-12</td>
    <td>Not support WriteString(string) method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.Get("http://server/sample.csv");
    csvdoc.Load(res);
    var fs = new FileSystem;
    var fp = fs.Open("sample.csv", FileSystem.OPEN_WRITE);
    csvdoc.Save(fp);
    fp.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a> method</td>
  </tr>
</table>



