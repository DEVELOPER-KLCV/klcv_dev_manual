---
layout: default

parent: 3. Extension3 Package
has_children: true

title: TreeView Class
nav_order: 7
permalink: /package/extension3/treeview

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext3-TreeView.PNG" target="_blank">
<img src="/img/Package/Ext3-TreeView.PNG" alt="login image"></a>

A class that displays a tree view.

The TreeView class works in tandem with the TreeItem class.

To set the data to be displayed as a tree item, it is necessary to place an object of the TreeItem class or its derived class in the structure defined under the TreeView object.

Since ver5.0, the STree class that makes the tree view easier to handle has been added. The STree class can display a tree structure that is easier to handle than the tree view of this class.

**Object Structure**

<a href="/img/Package/Ext3-TreeView1.PNG" target="_blank">
<img src="/img/Package/Ext3-TreeView1.PNG" alt="login image"></a>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image002.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

### **Specifying Icon Number**

By default, the displayed icon types are as follows.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Icon No</th>
    <th class="tg-kg9c">Icon Image</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">0 ～ 9</td>
    <td class="tg-0pky"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image003.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0pky">10 ～ 19</td>
    <td class="tg-0pky"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image004.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0lax">20 ～ 29</td>
    <td class="tg-0lax"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image005.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0lax">30 ～ 39</td>
    <td class="tg-0lax"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image006.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0lax">40 ～ 49</td>
    <td class="tg-0lax"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image007.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0lax">50 ～ 59</td>
    <td class="tg-0lax"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image008.gif" width="178" height="16"></td>
  </tr>
  <tr>
    <td class="tg-0lax">60</td>
    <td class="tg-0lax"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext6.files/image009.gif" width="16" height="16"></td>
  </tr>
</tbody>
</table>

<a href="/package/extension3/treeview/methods/setimage">SetImage</a> method can be used to change to the icon stored in the <a href="/package/extension4/imagelist//methods/imagelist">ImageList</a> object.

**Printer output by Doc class**<br>
 Not subject to printing.

**Default properties and ValueType**<br>
 The default property is <a href="/package/extension3/treeview/properties/value">Value</a>. The value type specification is invalid.
 
**Restrictions when visual style is enabled**<br>
Nothing in particular

 **Precautions when scaling**<br>
◆ The size of the tree display itself is only affected by the font size
