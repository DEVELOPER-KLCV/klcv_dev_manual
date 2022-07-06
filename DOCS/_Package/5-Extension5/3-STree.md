---
layout: default

parent: 5. Extension5 Package
has_children: true

title: STree Class
nav_order: 3
permalink: /package/extension5/stree

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}

<a href="/img/Package/Ext5-STree.PNG" target="_blank">
<img src="/img/Package/Ext5-STree.PNG" alt="login image"></a>

A class that displays a simple operation tree view. It provides a tree structure display that is easier to handle than the traditional <a href="/package/extension3/treeview">TreeView</a> class.

Use the STreeItem class to work with each tree item.

The STree class, unlike the TreeView class, has no corresponding object for each tree item. Like the FlexView class, individual tree items are managed as internal data in the STree class and must be manipulated through the <a href="/package/extension5/streeitem">STreeItem</a> class.

Tree items are created with the Append method of the STreeItem class. In addition to the method of adding one item by specifying a character string, you can also specify XML to generate a tree structure in a batch.

Example<br>
```
var rootitem = STree1.RootItem;
var item1 = rootitem.Append("item1");
 
var xdoc = new XmlDocument();
xdoc << xml <<-
<?xml version="1.0" encoding="SHIFT_JIS"?>
<data>
    <item title="item2">
        <item title="item2-1"/>
        <item title="item2-2"/>
    </item>
</data>
->>;
var item2 = rootitem.Append(xdoc);
```

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext5/ext_stree.files/image001.jpg" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
Not subject to printing.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension5/stree/properties/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.

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

The <a href="/package/extension5/stree/methods/setimage">SetImage</a> method can be used to change to the icon stored in the <a href="/package/extension4/imagelist">ImageList</a> object.

**Accessor object**<br>
Tree items are not objects, so you cannot work with individual tree items directly, but the STreeItem class is defined as an accessor to tree items. An accessor is a kind of pointer, and operations to the accessor are transmitted to the tree item pointed to by the accessor. For example, if you change the accessor of the tree item obtained from the STree class, the Title of the STreeItem, the display string of the tree item pointed to by the STreeItem will change.

Since the accessor is not the tree item itself, the states of the accessor and the tree item are not always in sync. For example, if you define two accessors for one tree item and call the Delete method of one accessor to delete it, the other accessor will not be deleted and will be an invalid accessor pointing to an item that does not exist.

 
**Scope of use of accessors**<br>
Accessors are created dependent on the source STree object and the parent tree item, and work with the internal STreeItem object to actually access the tree item. Therefore, the accessor object cannot work if the STree object is lost or the parent tree item is deleted. If you use accessors, be sure to maintain STree objects and parent tree items. It is not necessary to maintain the accessor for the parent tree item.

 
**About accessors and object trees**<br>
The object tree represents the hierarchical relationships between objects in the CRS language. On the other hand , the hierarchical structure of tree items in the STree class is managed inside STree, not as the hierarchical structure of objects . Therefore, it is not possible to search for a tree item using the FindObject method or FindChild method for the STreeItem object that is the accessor. Use <a href="/package/extension5/stree/methods/finditem">FindItem</a> and <a href="/package/extension5/stree/methods/finditems">FindItems</a> methods to search for tree items .


**FirstVisibleItem and LastVisibleItem**<br>The <a href="/package/extension5/stree/properties/firstvisibleitem">FirstVisibleItem</a> property refers to the item displayed at the top of the screen according to the scroll position, such as the item surrounded by the red frame in the figure below.

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext5/ext_stree.files/image009.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

On the other hand, please note that the <a href="/package/extension5/stree/properties/lastvisibleitem">LastVisibleItem</a> property points to the object displayed at the bottom regardless of the scroll position, as shown in the figure below.

<a href="/img/Package/Ext5-STree1.PNG" target="_blank">
<img src="/img/Package/Ext5-STree1.PNG" alt="login image"></a>

**Restrictions when visual style is enabled**<br>
Nothing in particular

**Precautions when scaling**<br>
◆ The size of the tree display itself is only affected by the font size