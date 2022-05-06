---
layout: default

grand_parent: TrayIcon Class
parent: Methods
has_children: false
title: TrayIcon.SetImage Method
nav_order: 4
permalink: /package/extension4/trayicon/methods/SetImage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TrayIcon1.SetImage( <b>img</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ImageList <b>img</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ImageList iconImage {
        MaskUse = $TRUE;
        MaskColB = 255;
        MaskColR = 255;
        LoadImage("icon.png");
    }
    TrayIcon1.SetImage(iconImage);
    TrayIcon1.Icon = 1;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/trayicon/property/Icon">Icon</a> property<br><a href="/package/extension4/trayicon/methods/ResetImage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>