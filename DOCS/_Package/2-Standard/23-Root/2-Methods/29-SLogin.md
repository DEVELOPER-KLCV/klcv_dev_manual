---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SLogin Property
nav_order: 29
permalink: /package/standard/root/methods/slogin
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Log in to the specified server in single session mode.<br><br>All current sessions will be disconnected and all existing objects will be deleted. Since Biz / Browser is initialized by calling the SLogin method, the CRS program described after the SLogin method will not be executed. Describe the operation after login in the CRS program specified in the <b><i>URL</i></b>. 
    
    <br><br><b><i>Single Session Mode</i></b><br>
    While the session started by the SLogin method is valid, Biz / Browser will be in single session mode and will not be able to communicate with servers other than the connection destination specified in the <b><i>URL</i></b>. <br>Also, even if an exception that is not trapped occurs during single session mode, the debug information (core dump) will not be output.
    
    <br><br>These restrictions are provided for applications that require a high degree of security, and when used in combination with the <a href="/package/httppackage/httpsession/methods/isloginsession">HttpSession.IsLoginSession</a> method, it is possible to prevent the application from loading unintended CRS programs at the same time.

    <br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SLogin( <b>URL</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URL</b></td>
    <td>Destination URL<br> Unlike the <a href="/package/standard/root/methods/login">Login</a> method, the connection destination is specified collectively by URL instead of specifying Server and URI individually.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var session = getHttpSession();
    if (session.IsLoginSession($TRUE)) {
        //.Get("main.crs");
    } else {
        //.SLogin("https://server/login.crs");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/login">Login</a>, <a href="/package/standard/root/methods/logout">Logout</a> methods<br><a href="/package/httppackage/httpsession/methods/isloginsession">HttpSession.IsLoginSession</a> method</td>
  </tr>
</table>



