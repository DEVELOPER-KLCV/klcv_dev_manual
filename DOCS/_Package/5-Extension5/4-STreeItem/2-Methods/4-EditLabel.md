---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.EditLabel Method
nav_order: 4
permalink: /package/extension5/streeitem/methods/editlabel
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Start editing the title of the item. <br>If the Active property of the STree object to which it belongs is $FALSE or the Editable property is $FALSE, nothing is done.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.EditLabel()</td>
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
    <td rowspan="2">Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
  </tr>
  <tr>
    <td>EXT-22</td>
    <td>This operation cannot be performed on RootItem</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    STree1.RootItem.Child.EditLabel();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>