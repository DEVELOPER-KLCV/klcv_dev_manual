---
layout: default

grand_parent: JSONDocument Class
parent: Methods
has_children: false
title: JSONDocument.Parse Method
nav_order: 3
permalink: /package/jsonpackage/jsondocument/methods/parse
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Read JSON data from a string .<br><br>The Value value before executing the Parse method will lost.<br><br>The Parse method has the same loading function as the <a href="/package/jsonpackage/jsondocument/methods/load">Load</a> method, but you can specify a String or UString object as an argument .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">jsondoc.Parse (<b><i>str</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td>String (UString) <b><i>str</i></b></td>
    <td>JSON string</td>
  </tr>
 <tr>
    <td>Exception</td>
    <td>JSON-1</td>
    <td>Nth character analysis failed</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
        var jsondoc = new JSONDocument;
        var str = "[{\" aaa \ ": \" bbb \ "}, \" ccc \ "]";
        jsondoc.Parse (str);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/jsonpackage/jsondocument/methods/save">Save</a>, <a href="package/jsonpackage/jsondocument/methods/get">Get</a>, <a href="/package/jsonpackage/jsondocument/methods/load">Load</a> methods</td>
  </tr>
</table>