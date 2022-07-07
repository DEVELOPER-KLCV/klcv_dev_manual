---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.DeleteChild Method
nav_order: 3
permalink: /package/extension5/streeitem/methods/deletechild
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Disconnects all child objects connected to the object from the object tree.<br> See the <a href="/package/extension5/streeitem/methods/delete">Delete</a> method for disconnecting from the object tree.<br><small><span style="color:green">Since Ver.5.0.2, in addition to the above, it has been extended to delete its own child items from the tree.</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.DeleteChild()</td>
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
    STree1.RootItem.DeleteChild();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/object/methods/deletechild">Object.DeleteChild</a> method</td>
  </tr>
</table>