---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.FindItem Method
nav_order: 7
permalink: /package/extension5/streeitem/methods/finditem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.FindItem( <b>data</b> [, <b>option</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>data</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>option</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var foundItem = STree1.RootItem.FindItem("abc");
    if (foundItem != null) {
        MessageBox("タイトルが'abc'のアイテムが見つかりました。");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/methods/finditems">FindItems</a> method</td>
  </tr>
</table>
