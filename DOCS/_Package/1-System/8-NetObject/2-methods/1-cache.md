---
layout: default

grand_parent: NetObject Class
parent: Methods
has_children: false
title: NetObject.Cache Method
nav_order: 1
permalink: /package/system/netobject/methods/cache
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Download the CRS file from the WEB server and cache it.<br><br>It works the same as the Get method , except that it doesn't run the downloaded CRS. See the <a href="/package/system/netobject/methods/get">Get</a> method for details. <br><br> If "Do not use cache" is set in the Biz / Browser environment settings, it will not be cached. Also, if the cache prohibition attribute is added to the response header from the server or the time stamp is unknown, it will not be cached.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Cache (<b>URL [, param1 [, param2 [, ...]]]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL of the CRS file<br>Same as the <b>URL</b> of the Get method</td>
  </tr>
  <tr>
    <td>Object <b>param</b></td>
    <td>Parameters to be added to the request<br>Same as the <b>param</b> of Get method.<br><br>A general WEB server adds a cache prohibition attribute to the response header of a POST request with parameters. When using <b>param</b> , it is necessary to consider the behavior of such a WEB server.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CRS-331</td>
    <td>Communication error<br>Same as the Get method exception.</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function LoadCache() {
    //.Cache("Form1.crs");
    //.Cache("Form2.crs");
    //.Cache("Form3.crs");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a>Get</a> method<br><a>Root.CacheSetup</a> method<br><a>Root.CacheMode</a> property</td>
  </tr>
</table>



