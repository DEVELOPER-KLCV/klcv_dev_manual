---
layout: default

grand_parent: NetObject Class
parent: Methods
has_children: false
title: NetObject.Get Method
nav_order: 3
permalink: /package/system/netobject/methods/get
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Get( <b>URL</b> [, <b>param1</b> [, <b>param2</b> [, ... ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>URL</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Object <b>param</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CRS-331</td>
    <td>Communication error<br>The Exception object has the following structure.<br><code><pre>Exception {
    String RequestURL;  /* URL of the request that caused the exception */
    Number StatusCode;  /* HTTP status code */
    String ContentType; /* Content-Type of HTTP header */
    String Body;        /* Response body */
}</pre></code></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnTouch(e) {
    //.Form1.Delete();
    //.Get("Form2.crs");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/netobject/methods/cache">Cache</a>, <a  href="/package/csvpackage/csvdocument/methods/get">CSVDocument.Get</a> methods</td>
  </tr>
</table>



