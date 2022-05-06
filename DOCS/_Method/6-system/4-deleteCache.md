---
layout: default

parent: 6. System Functions

title: deleteCache
nav_order: 4
permalink: /method/system/deleteCache
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the cache indicated by the URI. <br> <small>This function is left for compatibility with older versions, but is available. It is internally transferred to the call of the Root.DeleteCache method. In new programs, use the Root.DeleteCache method. <br> Unlike the conventional deleteCache function , the Root.DeleteCache method deletes the corresponding Internet Explorer cache entry at the same time when called during communication using IEConnect. </small>  </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">deleteCache ([<b>URI</b> ])</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URI</b></td>
    <td>Specifies the URI to delete. <br><br>If the URI is omitted, all caches from the server that downloaded the CRS file that called the deleteCache function will be deleted. <br><br> If * (asterisk) is specified at the end of the URI, all prefix-matching URLs will be deleted. Since the cache to be deleted is determined by the prefix match in the URL string comparison, the directory name and file name are not distinguished. <small> Added since Mobile Ver.3.0.0 </small> <br><br> The URI cannot specify the protocol and host name, and if included, it will be ignored. Therefore, it is not possible to delete the cache generated from a server other than the server that downloaded the CRS file that called the deleteCache function. This is a constraint designed to prevent unintentional deletion of the cache used by another application. <br> One thing to note about this constraint is the cache control of the image file. Image files loaded by URL into SVG, ImageLabel, etc. are also cached, but if the image file is downloaded from a server different from the application, there is no way to remove the cache of that image file from the script.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>deleteCache ("/app1/form1.crs");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/cachedate">cachedate</a> function <br> <a href="/method/statistical/Root.DeleteCache">Root.DeleteCache</a> method</td>
  </tr>
</table>





