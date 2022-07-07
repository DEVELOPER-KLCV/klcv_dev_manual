---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.Insert Method
nav_order: 9
permalink: /package/extension5/streeitem/methods/insert
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add the item before the node.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.Insert( <b><i>title</i></b> )<br>OR<br>item.Insert( <b><i>xmlDoc</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">STreeItem object<br> If pass a string as an argument, it returns the accessor for the added item. If pass an XMLDocument object as an argument, it returns the first object added.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>title</i></b></td>
    <td>Character string to be set in the Title property of the item to be added</td>
  </tr>
  <tr>
    <td><b><i>xmlDoc</i></b></td>
    <td><a href="/package/xmlpackage/xmldocument">XmlDocument</a> object with a <a href="/package/extension5/streeitem/#format-for-adding-items-by-passing-an-xml-document-">Specific Format</a><br>XmlDocument with <a href="/package/xmlpackage/xmldomimplementation/methods/constructor#about-xml-with-a-unicode-internal-character-code">Unicode internal character code</a> cannot be specified.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var item = STree1.RootItem.Child;
    item.Insert("abc");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/methods/append">Append</a>, <a href="/package/extension5/streeitem/methods/delete">Delete</a> methods</td>
  </tr>
</table>
