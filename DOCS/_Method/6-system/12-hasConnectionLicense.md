---
layout: default

parent: 6. System Functions

title: hasConnectionLicense
nav_order: 12
permalink: /method/system/hasConnectionLicense
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Check if a [connection license]() is registered for the connection destination Web server indicated by the <b>URL</b>. <br>Connection license verification is identified by the <b>URL</b> protocol name (http, https, etc.), host name, and port number string (http://example.com:8080, etc.). There are various notations that represent the same connection destination, such as the direct notation of the IP address and the alias of the host name, but only the notation that matches the Web server information described in the [connection license certificate]() is valid. <br> <small> Added from Ver.4.1.0 and Mobile Ver.2.0.0</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var flag = hasConnectionLicense(<b>URL</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$ TRUE is returned if a connection license to the <b>URL</b> is registered, otherwise$ FALSE is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL of the connected web server to check</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>if (! hasConnectionLicense ("http: // server")) {
    importConnectionLicese ("http://server/License.xml");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/importConnectionLicense">importConnectionLicense</a> function</td>
  </tr>
</table>





