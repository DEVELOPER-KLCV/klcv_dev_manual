---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.GetChildItems Methods
nav_order: 2
permalink: /package/extension3/treeview/methods/getchilditems
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the child's tree item.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var items = TreeView1.GetChildItems( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"><a href="/package/system/array">Array</a> object containing <a href="/package/extension3/treeitem">TreeItem</a> object</td>
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
    <td colspan="2"><code><pre>
    if (TreeView1.HasChildItems()) {
        var items = TreeView1.GetChildItems();
        for (var i = 0; i < items.Length; i++) {
            var item = items[i];
            print(item.Name, "\n");
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension3/treeview/methods/haschilditems">HasChildItems</a> method<br><a href="/package/system/array">Array</a>, <a href="/package/extension3/treeitem">TreeItem</a> class<br><a href="/package/extension3/treeitem/methods/getchilditems">TreeItem.GetChildItems</a> method</td>
  </tr>
</table>