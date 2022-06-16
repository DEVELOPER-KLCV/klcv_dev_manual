---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.SetImage Methods
nav_order: 6
permalink: /package/extension3/treeview/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets the image list used to display the icon of the tree item.<br><small><span style="color:red">Added since Ver.4.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TreeView1.SetImage( <b><i>img</i></b> )</td>
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
    <td>EXT-5</td>
    <td>ImageList reference is abnormal</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TreeView1.SetImage(ImageList1);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension3/treeitem/properties/closeicon">TreeItem.CloseIcon</a>, <a href="/package/extension3/treeitem/properties/openicon">TreeItem.OpenIcon</a> properties<br><a href="/package/extension3/treeview/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>