---
layout: default

grand_parent: ListView Class
parent: Methods
has_children: false
title: ListView.SetLargeImage Method
nav_order: 7
permalink: /package/extension4/listview/methods/setlargeimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the image list used for displaying large icons.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ListView1.SetLargeImage( <b><i>img</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ImageList <b><i>img</i></b></td>
    <td><a href="/package/extension-4/imagelist">ImageList</a> object that holds the image list you want to display</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td>ImageList reference is abnormal</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ListView1.SetLargeImage(ImageList1);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/listviewitem/properties/icon">ListViewItem.Icon</a> property<br><a href="/package/extension4/listview/methods/resetlargeimage">ResetLargeImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>