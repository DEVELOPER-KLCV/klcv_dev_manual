---
layout: default

grand_parent: TrayIcon Class
parent: Methods
has_children: false
title: TrayIcon.SetIcon Method
nav_order: 3
permalink: /package/extension4/trayicon/methods/seticon
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the icon file (* .ico) used to display the icon in the task tray.<br><small><span style="color:red">Added since Ver.5.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TrayIcon1.SetIcon( <b><i>URL or reader</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b><i>URL or reader</i></b></td>
    <td>URL or <a href="/base/readerwriter#reader-object">ReaderObject</a></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-59</td>
    <td>The argument of SetIcon is invalid</td>
  </tr>
  <tr>
    <td>EXT-60</td>
    <td>Unable to create temporary file</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TrayIcon1.SetIcon("/image/window.ico");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/trayicon/methods/reseticon">ResetIcon</a> method</td>
  </tr>
</table>