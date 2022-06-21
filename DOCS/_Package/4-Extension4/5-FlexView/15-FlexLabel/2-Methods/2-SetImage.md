---
layout: default

grand_parent: FlexLabel Class
parent: Methods
has_children: false
title: FlexLabel.SetImage Method
nav_order: 2
permalink: /package/extension4/flexview/flexlabel/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the image list used to display the cell icon.<br>

 

Display example<br>

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlabelm1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>
<br>
If the icon displayed is larger than the row height, it will be scaled down while maintaining the aspect ratio.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">FlexLabel1.SetImage( <b><i>img</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ImageList <b><i>img</i></b></td>
    <td><a href="/package/extension4/imagelist">ImageList</a> object that holds the image list you want to display</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    FlexLabel FlexLabel1 {
        :
    }
    var img = new ImageList {
        MaskUse = $TRUE;
        MaskColR = 1;
        LoadIcon("crs");
        LoadIcon("bdp");
        LoadIcon("car");
    }
    FlexLabel1.SetImage(img);
    FlexLabel1.Icon = 0;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/flexview/flexlabel/properties/icon">Icon</a> property<br><a href="/package/extension4/flexview/flexlabel/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class<br></td>
  </tr>
</table>