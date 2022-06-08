---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetIcon Property
nav_order: 22
permalink: /package/standard/root/methods/seticon
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the icon file ( * .ico ) used to display the icon of the window title.<br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetIcon( <b>URL or reader</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or reader</b></td>
    <td>URL or <a href="/base/readerwriter#reader-object">ReaderObject</a></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>PKG-59</td>
    <td>The argument of SetIcon is invalid</td>
  </tr>
  <tr>
    <td>PKG-60</td>
    <td>Unable to create temporary file</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetIcon("/image/window.ico");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/reseticon">ResetIcon</a> method</td>
  </tr>
</table>



