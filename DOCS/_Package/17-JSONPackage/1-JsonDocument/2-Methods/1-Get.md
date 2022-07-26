---
layout: default

grand_parent: JSONDocument Class
parent: Methods
has_children: false
title: JSONDocument.Get Method
nav_order: 1
permalink: /package/jsonpackage/jsondocument/methods/get
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Reads JSON data from the specified URL .<br><br>The Value value before executing the Get method is lost.<br>The JSON data to be acquired is not cached. Always get from the server.<br><br>If you do not specify <b><i>param</i></b> , thebe sentHTTPGET.<br>If you specify <b><i>param</i></b> , thebe sentHTTPPOST<br><br>If the web server does not return 200 ( $HTTP_OK ) for the HTTP status code, a CRS-331 exception will occur.<br><br>If the internal character code is Unicode , the character code of the input JSON file is UTF-8 </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">jsondoc.Get( <b><i>URL</i></b> [, <b><i>param1</i></b> [, <b><i>param2</i></b>, … ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Argument</td>
    <td>String <b><i>URL</i></b></td>
    <td>URL to read JSON data<br>Same as the <b><i>URL</i></b> of the NetObject.Get method.</td>
  </tr>
   <tr>
    <td>Object <b><i>param</i></b></td>
    <td>Parameters to be added to the request<br>Same as <b><i>param</i></b> of NetObject.Get method.</td>
  </tr>
 <tr>
    <td rowspan="2">Exception</td>
    <td>JSON-1</td>
    <td>Nth character analysis failed</td>
  </tr>
  <tr>
    <td>CRS-331</td>
    <td>Communication error<br>Same as the exception to the NetObject.Get method.</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var jsondoc = new JSONDocument;
    jsondoc.Get("/test/sample.cgi", "KEY=126", "MODE=A");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/jsonpackage/jsondocument/methods/load">Load</a>, <a href="/package/jsonpackage/jsondocument/methods/parse">Parse</a>, <a href="/package/system/netobject/methods/get">NetObject.Get</a> methods</td>
  </tr>
</table>
