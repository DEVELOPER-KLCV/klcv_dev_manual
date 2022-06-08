---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.DeleteCache Property
nav_order: 4
permalink: /package/standard/root/methods/deletecache
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the cache indicated by the <b><i>URI</i></b>. <br><br>It is not possible to delete a cache generated from a server other than the one that downloaded the CRS file that called the DeleteCache method. The <b><i>URI</i></b> cannot specify the protocol (http: //) and host name, and even if it is included, it will be ignored. This is a constraint designed to prevent unintentional deletion of the cache used by another application.<br><br>One thing to note about this constraint is the cache control of the image file. Image files loaded by URL into ImageLabel objects etc. are also cached, but if the image file is downloaded from a server different from the application, there is no way to remove the cache of that image file from the script. </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.DeleteCache( [ <b>URI</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URI</b></td>
    <td>Specify the URI to delete.<br>If omitted, all caches from the server that downloaded the CRS file that called the DeleteCache method will be deleted.<br><br>If * (asterisk) is specified at the end of the URI, all prefix-matching URLs will be deleted. The cache to be deleted is determined by the prefix match in the character string comparison of the URL, so the directory name and file name are not distinguished.<br><small><span style="color:red">Added since Ver.4.0.0, Mobile Ver.3.0.0</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.DeleteCache("/app1/form1.crs");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/cachedate">cachedate</a> method</td>
  </tr>
</table>



