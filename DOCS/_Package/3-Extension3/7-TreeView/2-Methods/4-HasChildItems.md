---
layout: default

grand_parent: TreeView Class
parent: Methods
has_children: false
title: TreeView.HasChildItems Methods
nav_order: 4
permalink: /package/extension3/treeview/methods/haschilditems
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Check for children's tree items.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = TreeView1.HasChildItems( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns $ TRUE if there are children's tree items, $ FALSE otherwise.</td>
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
        TreeView1.GetChildItems();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension3/treeview/methods/getchilditems">GetChildItems</a> method<br><a href="/package/extension3/treeitem/methods/haschilditems">TreeItem.HasChildItems</a> method</td>
  </tr>
</table>