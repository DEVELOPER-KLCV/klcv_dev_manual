---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.CreateItem Methods
nav_order: 1
permalink: /package/extension3/TreeView/methods/CreateItem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var item = TreeView1.CreateItem( [ <b>name</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TreeView TreeView1 {
        :
        TreeItem TreeItem1;
        :
        Function addItem() {
            var item = CreateItem("abc");
            item.Title = "new item";
            TreeItem1.Append(item);
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension3/TreeItem">TreeItem</a> class<br><a href="/package/system/object/methods/append">Object.Append</a> method</td>
  </tr>
</table>