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
    <td colspan="2">Add the item to the end of own child.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.Append( <b><i>title</i></b> )<br>OR<br>item.Append( <b><i>xmlDoc</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">STreeItem object<br>If you pass a string as an argument, it returns the accessor for the added item.<br> If you pass an XMLDocument object as an argument, it returns the first object added.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>title</i></b></td>
    <td>Character string to be set in the  <a href="/package/extension5/streeitem/properties/title">Title</a> property of the item to be added</td>
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
