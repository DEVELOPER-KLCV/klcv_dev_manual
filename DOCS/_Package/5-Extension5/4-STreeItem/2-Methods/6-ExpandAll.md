---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.ExpandAll Method
nav_order: 6
permalink: /package/extension5/streeitem/methods/expandall
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Expand and collapse the tree in bulk include all its descendants.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.ExpandAll( [ <b>expanded</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>expanded</b></td>
    <td>If $TRUE is specified, the tree will be expanded. <br> If $FALSE is specified, it collapses the tree. The default is $TRUE.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var foundItems = STree1.RootItem.ExpandAll();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/properties/expanded">Expanded</a> property</td>
  </tr>
</table>
