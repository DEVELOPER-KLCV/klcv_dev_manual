---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.Login Property
nav_order: 11
permalink: /package/standard/root/methods/login
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Log in to the specified server.<br><br>	For login, refer to the <a href="/bizBrowserV/4/4-4/">behavior when logging in to Biz / Browser</a>. If all parameters are omitted, the login screen will be displayed.<br><br>All current sessions will be disconnected and all existing objects will be deleted.Since Biz / Browser is initialized by calling the Login method, the CRS program described after the Login method will not be executed.Describe the operation after login in the CRS program specified in the <b><i>URI</i></b>.
 </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.Login( [ <b>server</b> [, <b>URI</b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>server</b></td>
    <td>Connection destination server URL</td>
  </tr>
  <tr>
    <td>String <b>URI</b></td>
    <td>Path of resource to connect</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    Login("http://server1:81", "/app1/mainmenu.crs");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/logout">Logout</a>, <a href="/package/standard/root/methods/slogin">SLogin</a> methods</td>
  </tr>
</table>



