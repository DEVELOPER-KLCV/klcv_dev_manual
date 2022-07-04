---
layout: default

grand_parent: TrayIcon Class
parent: Methods
has_children: false
title: TrayIcon.SetImage Method
nav_order: 4
permalink: /package/extension4/trayicon/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the image list used to display the icon in the task tray.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TrayIcon1.SetImage( <b><i>img</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ImageList <b><i>img</i></b> </td>
    <td><br><a href="/package/extension4/imagelist">ImageList</a> object that holds the image list you want to display</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td>ImageList reference is abnormal</td>
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
    <td colspan="2"><a href="/package/extension4/trayicon/property/icon">Icon</a> property<br><a href="/package/extension4/trayicon/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>