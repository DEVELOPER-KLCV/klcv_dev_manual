---
layout: default

grand_parent: 5. Extension5 Package
parent: STreeItem Class

title: Properties
nav_order: 1
permalink: /package/extension5/streeitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the STreeItem class.

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
|[Child](/package/extension5/streeitem/properties/child) | R | STreeItem |  Accessor for the item of its first child|
|[CloseIcon](/package/extension5/streeitem/properties/closeicon) | CRW | integer | Icon with the tree closed |
|[Expanded](/package/extension5/streeitem/properties/expanded) | CRW | boolean | Expand / collapse state of the item tree |
|[Id](/package/extension5/streeitem/properties/id) | R | integer | Item ID|
|[Next](/package/extension5/streeitem/properties/next) | R | STreeItem |Accessor for its next item |
|[NextVisible](/package/extension5/streeitem/properties/nextvisible) | R | STreeItem |Accessor of the item displayed next to itself |
|[OpenIcon](/package/extension5/streeitem/properties/openicon) | CRW | integer |Icon when the tree expanded |
|[Parent](/package/extension5/streeitem/properties/parent) | R | STreeItem |Accessor of own parent's item |
|[Prev](/package/extension5/streeitem/properties/prev) | R | STreeItem |Accessor of the previous item |
|[PrevVisible](/package/extension5/streeitem/properties/prevvisible) | R | STreeItem | Accessor of the previously displayed item |
|[Selected](/package/extension5/streeitem/properties/selected) | CRW | boolean |Item selection status |
|[Title](/package/extension5/streeitem/properties/title) | CRW | String | Item display character|
|[Value](/package/extension5/streeitem/properties/value)* | CRW | String |Object value |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property