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
    <td colspan="2"></td>
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
    <td></td>
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



