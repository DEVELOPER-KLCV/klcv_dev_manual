---
layout: default

grand_parent: FlexHeader Class
parent: Methods
has_children: false
title: FlexHeader.SetImage Method
nav_order: 2
permalink: /package/extension4/flexview/flexheader/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">FlexHeader1.SetImage( <b>img</b> )</td>
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
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    FlexHeader FlexHeader1 {
        :
    }
    var img = new ImageList {
        MaskUse = $TRUE;
        MaskColR = 1;
        LoadIcon("crs");
        LoadIcon("bdp");
        LoadIcon("car");
    }
    FlexHeader1.SetImage(img);
    FlexHeader1.Icon = 0;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/flexview/flexheader/properties/icon">Icon</a> property<br><a href="/package/extension4/flexview/flexheader/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class<br></td>
  </tr>
</table>