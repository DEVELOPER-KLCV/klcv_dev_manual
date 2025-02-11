---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.Delete Method
nav_order: 2
permalink: /package/extension5/streeitem/methods/delete
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes itself and all items pointed to by its children. <br>When called for a root item, it deletes all items except the root item. <br>The accessor indicating the deleted item is disabled and the <a href="/package/extension5/streeitem/properties/id">Id</a> property is 0.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.Delete( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    STree1.RootItem.Delete();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/methods/append">Append</a>, <a href="/package/extension5/streeitem/methods/insert">Insert</a> methods</td>
  </tr>
</table>
