---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.ShowStatusBar Property
nav_order: 28
permalink: /package/standard/root/methods/showstatusbar
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specifies whether to show or hide the status bar of the root window.<br><br>The status bar is displayed in the initial state immediately after startup. It returns to the initial state when the <a href="/package/standard/root/methods/login">Login</a> and <a href="/package/standard/root/methods/logout">Logout</a> methods are executed. This method does nothing if Biz / Browser is running inside Internet Explorer.<br><small><span style="color:red">Added since Ver.5.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.ShowStatusBar( <b>flag</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>flag</b></td>
    <td>If specify $ TRUE, the status bar will be displayed.<br>If specify $ FALSE, the status bar will be hidden.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.ShowStatusBar($FALSE);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/showmenu">ShowMenu</a> method</td>
  </tr>
</table>



