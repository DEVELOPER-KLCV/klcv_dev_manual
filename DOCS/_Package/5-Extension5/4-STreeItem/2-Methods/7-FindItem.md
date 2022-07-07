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
    <td colspan="2">Recursively searches for items in its own child and returns the accessor for the first item found.<br> It is not included in the search target.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.FindItem( <b><i>data</i></b> [, <b><i>option</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">An STreeItem object that serves as an accessor to the first item found. <br>If it cannot be found, it returns null.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>data</i></b></td>
    <td>Specify the character string to be searched. <br>Returns an object with properties that match this value. <br> Which property to compare with is specified by <b><i>option</i></b>.</td>
  </tr>
  <tr>
    <td><b><i>option</i></b></td>
    <td>Specify the property to be searched.  <br> Specify a combination of the following constants. <br>The default is STreeItem.FIND_VALUE. <br> If 0 is specified, null is returned as the return value.<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">STreeItem.FIND_TITLE</td>
    <td class="tg-j5n6">Compare<span style="font-weight:bold;font-style:italic"> data</span> and <a href="/package/extension5/streeitem/properties/title">Title</a> properties</td>
  </tr>
  <tr>
    <td class="tg-j5n6">STreeItem.FIND_VALUE</td>
    <td class="tg-j5n6">Compare <span style="font-weight:bold;font-style:italic">data</span> and <a href="/package/extension5/streeitem/properties/value">Value</a> properties</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
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
