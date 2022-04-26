---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.GetChildItems Methods
nav_order: 2
permalink: /package/extension3/TreeView/methods/GetChildItems
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var items = TreeView1.GetChildItems( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
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
    <td colspan="2"><a href="/package/extension3/TreeView/methods/HasChildItems">HasChildItems</a> method<br><a href="/package/system/Array">Array</a>, <a href="/package/extension3/TreeItem">TreeItem</a> class<br><a href="/package/extension3/treeitem/methods/GetChildItems">TreeItem.GetChildItems</a> method</td>
  </tr>
</table>