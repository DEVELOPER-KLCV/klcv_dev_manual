---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.Logout Property
nav_order: 12
permalink: /package/standard/root/methods/logout
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Log out and display the login screen.<br><br>All current sessions will be disconnected and all existing objects will be deleted. Since Biz / Browser is initialized by calling the Logout method, the CRS program described after the Logout method will not be executed.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.Logout( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    Function OnTouch(e) {
    //.Logout();
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/login">Login</a>, <a href="/package/standard/root/methods/slogin">SLogin</a> methods</td>
  </tr>
</table>



