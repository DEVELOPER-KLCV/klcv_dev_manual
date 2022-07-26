---
layout: default

grand_parent: JSONDocument Class
parent: Methods
has_children: false
title: JSONDocument.Load Method
nav_order: 2
permalink: /package/jsonpackage/jsondocument/methods/load
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Read JSON data from the Reader object .<br>The Value value before executing the Load method is lost.<br><br>If the internal character code is Unicode , the character code of the input JSON file is UTF-8 .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">jsondoc.Load( <b><i>reader</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td>Object <b><i>reader</i></b></td>
    <td><a href="/base/readerwriter#reader-object">ReaderObject</a> of read source ( object that can use Read method)</td>
  </tr>
 <tr>
    <td rowspan="3">Exception</td>
    <td>JSON-1</td>
    <td>Nth character analysis failed</td>
  </tr>
  <tr>
    <td>JSON-2</td>
    <td>No valid Read object specified</td>
  </tr>
    <tr>
    <td>JSON-3</td>
    <td>Does not support Read () method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
        var jsondoc = new JSONDocument;
        var res = session.get("/test/sample.json");
        jsondoc.Load(res);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/jsonpackage/jsondocument/methods/save">Save</a>, <a href="package/jsonpackage/jsondocument/methods/get">Get</a>, <a href="/package/jsonpackage/jsondocument/methods/parse">Parse</a> methods</td>
  </tr>
</table>