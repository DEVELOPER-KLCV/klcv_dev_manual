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
    <td colspan="2">Recursively searches for items of its own child and returns accessors for all found items in an Array object. <br>It is not included in the search target.<br><small><span style="color:green">The following specifications have been expanded since Ver.5.0.2--></span></small><br>If all arguments are omitted, the STreeItem object, which is an accessor to all its descendant items, is stored in the Array object and returned.<small><span style="color:green"><-- until here</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">item.FindItems( <b><i>data</i></b> [, <b><i>option</i></b> ] )<br><small><span style="color:green">It has been expanded since Ver.5.0.2 so that it can be called in the following format.</span></small><br>item.FindItems()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Stores and returns an STreeItem object that is an accessor to the found item in an Array object.<br> If it cannot be found, it returns an Array object with 0 elements.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>data</i></b></td>
    <td>Specify the character string to be searched. <br>Returns an object with properties that match this value. <br>Which property to compare with is specified by <b><i>option</i></b>.</td>
  </tr>
  <tr>
    <td><b><i>option</i></b></td>
    <td>Specify the property to be searched. <br>Specify a combination of the following constants. The default is STreeItem.FIND_VALUE.<br> If 0 is specified, all objects will not be searched.<br><style type="text/css">
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
