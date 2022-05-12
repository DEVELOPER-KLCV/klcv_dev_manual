---
layout: default

parent: 6. System Functions

title: importConnectionLicense
nav_order: 13
permalink: /method/system/importConnectionLicense
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">	Import the [connection license](). Download the [connection license certificate]() from the location indicated by the URL and register it in Biz / Browser. <br> The URL has nothing to do with the destination URLon the connection license certificate. The connection license certificate can be placed on any web server. <br> If a connection license with the same serial number as the connection license you are importing is already registered, the old one will be overwritten if the issue date is new, and an exception will be raised if the issue date is old. <br><small> Added from Ver.4.1.0 and Mobile Ver.2.0.0 </small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">importConnectionLicense (<b>URL</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL to download the license certificate file</td>
  </tr>
  <tr>
    <td rowspan="5">Exception</td>
    <td>CRS-394 </td>
    <td>The import URL is invalid</td>
  </tr>
  <tr>
    <td>CRS-396</td>
    <td>Connection to the designated server is restricted for security reasons</td>
  </tr>
  <tr>
    <td>CRS-331</td>
    <td>Communication error</td>
  </tr>
  <tr>
    <td>CRS-396</td>
    <td>The license certificate could not be recognized as a legitimate license</td>
  </tr>
  <tr>
    <td>CRS-399</td>
    <td>A newer license than the specified license certificate has already been registered</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>if (! hasConnectionLicense ("http: // server")) {
    importConnectionLicense ("http://server/License.xml");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/hasConnectionLicense">hasConnectionLicense</a> function</td>
  </tr>
</table>





