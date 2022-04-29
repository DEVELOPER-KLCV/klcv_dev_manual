---
layout: default

grand_parent: STreeItem Class
parent: Methods
has_children: false
title: STreeItem.Append Method
nav_order: 1
permalink: /package/extension5/streeitem/methods/append
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.Append( <b>title</b> )<br>OR<br>item.Append( <b>xmlDoc</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>title</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>xmlDoc</b></td>
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
    var parent = STree1.RootItem;
    var item_1 = parent.Append("abc");
    var item_2_1 = parent.Append("def").Append("ghi");
    
    var xmlDomImpl = new XmlDomImplementation;
    var xmlStr =
        "&lt;xml1> "+
        "  &lt;item title=\"def\" openicon=\"1\"/&gt;" +
        "  &lt;item title=\"ghi\" closeicon=\"2\"&gt;"+
        "    &lt;item title=\"hij\" closeicon=\"3\" openicon=\"4\" value=\"111\"&gt;" +
        "      &lt;item title=\"AAA\"/&gt;" +
        "      &lt;item title=\"BBB\"/&gt;" +
        "      &lt;item title=\"CCC\"/&gt;" +
        "    &lt;/item&gt;" +
        "    &lt;item title=\"klm\"/&gt;" +
        "  &lt;/item&gt;" +
        "&lt;/xml1&gt;";
    var xmlDoc = XmlDomImpl.Parse(xmlStr);
    var item_def = parent.Append(xmlDoc);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/streeitem/methods/delete">Delete</a>, <a href="/package/extension5/streeitem/methods/insert">Insert</a> methods</td>
  </tr>
</table>
