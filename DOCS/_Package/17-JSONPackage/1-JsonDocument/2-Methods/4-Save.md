---
layout: default

grand_parent: JSONDocument Class
parent: Methods
has_children: false
title: JSONDocument.Save Method
nav_order: 4
permalink: /package/jsonpackage/jsondocument/methods/save
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Output the Array object set to Value in the Writer object as JSON data.<br><br>If the Array object is not set in the Value value , "[]" is output.<br><br>Since CRS does not have a Boolean value internally, it will be <i>true</i> when saved and 1 or 0 when false .<br><br>If the internal character code is Unicode , the character code of the saved JSON file will be UTF-8 .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">jsondoc.Save( <b><i>writer</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td>Object <b><i>writer</i></b></td>
    <td><a href="/base/readerwriter#reader-object">WriterObject</a> to save to</td>
  </tr>
 <tr>
    <td rowspan="3">Exception</td>
    <td>JSON-4</td>
    <td>No valid Write object specified</td>
  </tr>
  <tr>
    <td>JSON-5</td>
    <td>Does not support the Write () method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
        var jsondoc = new JSONDocument;
        var res = session.Get("http://server/sample.json");
        jsondoc.Load(res);
        var fs = new FileSystem;
        var fp = fs.Open("sample.json", FileSystem.OPEN_WRITE);
        jsondoc.Save(fp);
        fp.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/jsonpackage/jsondocument/methods/load">Load</a> method</td>
  </tr>
</table>