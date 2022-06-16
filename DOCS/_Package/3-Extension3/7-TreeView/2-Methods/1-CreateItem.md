---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.CreateItem Methods
nav_order: 1
permalink: /package/extension3/treeview/methods/createitem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create a new tree item.<br>The created <a href="/package/extension4/treeitem/">TreeItem</a> object can be connected to any position in the tree by the <a href="/package/system/object/methods/append">Append</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var item = TreeView1.CreateItem( [ <b><i>name</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Created TreeItem object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>name</i></b></td>
    <td>Specifies the name of the TreeItem object to create. If omitted, it will be an anonymous object.</td>
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
    <td colspan="2"><a href="/package/extension3/treeitem">TreeItem</a> class<br><a href="/package/system/object/methods/append">Object.Append</a> method</td>
  </tr>
</table>