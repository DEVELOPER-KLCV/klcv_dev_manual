---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetBookmark Property
nav_order: 5
permalink: /package/standard/root/methods/getbookmark
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = //.GetBookmark( )</td>
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
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var list = //.GetBookmark();
for (var n = 0; n < list.length; n++) {
    print(list[n].url, list[n].title, "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/setbookmark">SetBookmark</a>, <a href="/package/standard/root/methods/rembookmark">RemBookmark</a> method</td>
  </tr>
</table>



