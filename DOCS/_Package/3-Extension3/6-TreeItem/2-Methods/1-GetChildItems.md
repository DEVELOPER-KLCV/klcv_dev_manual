---
layout: default

grand_parent: TreeItem Class
parent: Methods
has_children: false
title: TreeItem.GetChildItems Method
nav_order: 1
permalink: /package/extension3/treeitem/methods/getchilditems
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var items = TreeItem1.GetChildItems( )</td>
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
    Function ScanTreeItem(item) {
        print(item.Name, "\n");
        if (item.HasChildItems()) {
            var items = item.GetChildItems();
            for (var i = 0; i < items.Length; i++) {
                var titem = items[i];
                ScanTreeItem(titem);
            }
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension3/treeitem/methods/haschilditems">HasChildItems</a> method<br><a href="/package/system/array">Array</a> class</td>
  </tr>
</table>
