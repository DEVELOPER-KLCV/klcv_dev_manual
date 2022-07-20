---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Get Method
nav_order: 7
permalink: /package/csvpackage/csvdocument/methods/get
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Load CSV from specified URL.<br><br>The data before executing the Get method will be lost.<br>The CSV data to be acquired will not be cached. Always get from the server.<br><br>If not specify the <b><i>param</i></b>, request will be sent via HTTP GET.<br>If <b><i>param</i></b> is specified, request will be sent via HTTP POST.<br><br>If the web server does not return 200（$HTTP_OK）in HTTP status code, exception CRS-331 is thrown.<br><small><span style="color:red">Since Ver.4.0.5, Mobile Ver.3.0.0 it is possible to raise arbitrary exceptions using HTTP response headers. See <a href="/package/system/netobject/methods/get">NetObject.Get</a> for details.</span></small> <br><br><small><span style="color:red">From here added since Ver.4.2.0 --></span></small><br>If <a href="/package/csvpackage/csvdocument/methods/constructor#about-csvdocument-which-internal-character-code-is-unicodepc-ver-mobile-ver">About CSVDocument which internal character code is Unicode(PC ver, Mobile ver)</a>, character code for CSV file input will be Unicode.<br><small><span style="color:red"><--till here</span></small> <br><br><small><span style="color:green">Since AI Ver.1.0.1 changes are from here --></span></small><br>If WEB server does not specify charset in Content-type of HTTP Response Header, the received CSV data will be analysed as character string of the specified character code.<br><small><span style="color:green"><--till here</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Get( <b>URL [, param1 [, param2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String  <b>URL</b></td>
    <td>URL to read CSV data.<br>Same as the <b><i>URL</i></b> of the NetObject.Get method.</td>
  </tr>
  <tr>
    <td>Object <b>param</b></td>
    <td>Parameters to be added to the request<br>Same as <b><i>param</i></b> of NetObject.Get method</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>CSV-1</td>
    <td>CSV format is invalid</td>
  </tr>
  <tr>
    <td>CSV-10</td>
    <td>The number of columns is not constant</td>
  </tr>
  <tr>
    <td>CSV-331</td>
    <td>Communication error<br>Same excepetion as in NetObject.Get</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Get("/test/sample.cgi", "KEY=126", "MODE=A");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a>, <a href="/package/csvpackage/csvdocument/methods/parse">Parse</a>, <a href="/package/system/netobject/methods/get">NetObject.Get</a> methods</td>
  </tr>
</table>



