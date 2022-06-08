---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetDesktopWidth Property
nav_order: 7
permalink: /package/standard/root/methods/getdesktopwidth
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the horizontal size of the desktop. The size to be acquired is the part of the entire screen excluding the area occupied by the task bar of the system and the toolbar of the application. For Android version, returns the entire area (horizontal resolution of the display). In a multi-display environment, it is not possible to acquire screen sizes other than the primary monitor.<br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var width = //.GetDesktopWidth( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the vertical size of the desktop in pixels.</td>
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
    Form1.X = (//.GetDesktopWidth() - Form1.Width) / 2;
    Form1.Y = (//.GetDesktopHeight() - Form1.Height) / 2;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/getdesktopheight">GetDesktopHeight</a> method</td>
  </tr>
</table>



