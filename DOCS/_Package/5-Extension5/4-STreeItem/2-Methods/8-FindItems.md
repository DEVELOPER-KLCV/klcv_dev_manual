---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.FindItems Method
nav_order: 8
permalink: /package/extension5/streeitem/methods/finditems
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.FindItems( <b>data</b> [, <b>option</b> ] )<br><br>**<small>It has been extended from Version 5.0.2 so that it can be called in the following format.</small>**<br>item.FindItems()</td>
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
    var foundItems = STree1.RootItem.FindItems("abc");
    if (foundItems.Length != 0) {
        MessageBox("タイトルが'abc'のアイテムが" + str(foundItems.Length) + "個見つかりました。");
    }
    
    var allItems = STree1.RootItem.FindItems();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/methods/finditem">FindItem</a> method</td>
  </tr>
</table>
