---
layout: default

grand_parent: Dialog Class
parent: Methods
has_children: false
title: Dialog.SetIcon Method
nav_order: 3
permalink: /package/standard/dialog/methods/seticon
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the icon file ( * .ico ) used to display the icon of the dialog title.<br><small>Added since Ver 5.0.0<br>Not supported in Mobile, AI</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Dialog1.SetIcon( <b>URL or reader</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or reader</b></td>
    <td>URL or <a href="/base/readerwriter#reader-object">Reader</a></td>
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
    <td colspan="2"><code><pre>
Dialog1.SetIcon("/image/window.ico");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/dialog/methods/reseticon">ResetIcon</a> method</td>
  </tr>
</table>