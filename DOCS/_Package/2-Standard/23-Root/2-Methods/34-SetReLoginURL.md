---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetReLoginURL Property
nav_order: 34
permalink: /package/standard/root/methods/setreloginUrl
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specifies the URL to log in if the Biz / Browser AI process is automatically restarted after being forcibly terminated due to an external factor.<br> If no re-login destination is specified, it will be automatically logged in to the last logged-in CRS.<br><br> The re-login destination set by this method at the time of automatic restart is automatically set to the same one even after re-login, but it will be reset if the application is terminated normally or if you log in to a different CRS again.<br><br>If you want to save the data at a safe timing, save the data at the timing when $ ACTIVITY_ON_PAUSE of the WindowStateChanged event is received.<br><br>Please refer to the <a href="/bizBrowserV/2/2-5/">Android Version Features and Restrictions</a> for more information.<br><br><small><span style="color:red">Can only be use in AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetReloggedInURL( <b>URL</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URL</b></td>
    <td>Specify the URL of the login destination CRS with an absolute path.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetReloggedInURL("http://test.example.com/crs/relogin.crs");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/properties/reloggedin">ReLoggedIn</a> property</td>
  </tr>
</table>



