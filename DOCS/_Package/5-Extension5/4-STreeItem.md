---
layout: default

parent: 5. Extension5 Package
has_children: true

title: STreeItem Class
nav_order: 4
permalink: /package/extension5/streeitem

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}

<a href="/img/Package/Ext5-STreeItem.PNG" target="_blank">
<img src="/img/Package/Ext5-STreeItem.PNG" alt="login image"></a>

An accessor class for manipulating each item in the STree class. Be sure to get it from the <a href="/package/extension5/stree">STree</a>  class and use it.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension5/streeitem/properties/value">Value</a>. The value type specification is invalid.

### Format for adding items by passing an XML Document <br>
There are the following rules in XML when adding an item using an XMLDocument object with the <a href="/package/extension5/streeitem/methods/append">Append</a> and <a href="/package/extension5/streeitem/methods/insert">Insert</a> methods.

- The root node is skipped.
- The tag name will be skipped, so set any value.
- The corresponding properties can be set by setting values in the title, openicon, closeicon, and value attributes of the tag.
- When only one of the openicon and closeicon attributes is set, both openicon and closeicon have the same value.
- If a value is described in the value attribute, it will be set as a string type.

An example of XML description is shown below.

```
<xml><!-- 本タグは読み飛ばされる -->
  <item1 title="abc">
    <item11 title="def" openicon="1"/> <!-- openicon=closeicon=1; -->
    <item12 title="ghi" value="111"/>
    <item13 title="jkl" value="222>
      <item131 title="aaa"/>
        <item132 title="bbb"/>
      </item13>
    </item1>
    <item2 title="mno"/>
</xml>
```

When the above XML is specified in the Append method, the tree with the following structure is added as its own child, and the accessor of the object whose title is "abc" is the return value.

```
┌abc┬def
│　 ├ghi
│　 └jkl┬aaa
│　　　　└bbb
└mno
```

**Invalid Accessor**
 
If the item pointed to by the STreeItem object is deleted or the STree object to which the item belongs is deleted, the accessor becomes invalid and no further operations are accepted.

It can be determined if it is not an invalid accessor by checking if the [Id](/package/extension5/streeitem/properties/id)  property is non-zero. 


**Relationship of Next Visible and Next, Prev Visible and Prev**<br>
The <a href="/package/extension5/streeitem/properties/next">Next</a>  and  <a href="/package/extension5/streeitem/properties/prev">Prev</a>  properties refer to the previous and next items on their own hierarchy, while the  <a href="/package/extension5/streeitem/properties/nextvisible">NextVisible</a>  and  <a href="/package/extension5/streeitem/properties/prevvisible">PrevVisible</a>  properties refer to the previous and next items based on the display order of the screen.

The relationship between the Next property and the NextVisible property based on the selected item is as follows.

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext5/ext_streeitem.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

In addition, the relationship between the Prev property and the PrevVisible property based on the selected item is as follows.

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext5/ext_streeitem.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>


**Restriction of property setting by reference operator (& =)**
 
The "reference operator", which is an operator peculiar to Biz / Browser, automatically assigns the changed value to the left side when the right side of the assignment expression is changed.

(Example)

```
Width &= ^.Width - 10;
Height &= ^.Height - 10;
```

However, the properties of this class can make changes that cannot be detected by themselves by manipulating the STreeItem object that points to the same item.

When a reference operator is used for such a property, the processing target of the assignment destination (left side) and the value of the reference destination (right side) may differ depending on the state of other properties and objects, so it's difficult to get the intended result.

Therefore, **do not use** the STreeItem property on either the left or right side of the reference operator. 