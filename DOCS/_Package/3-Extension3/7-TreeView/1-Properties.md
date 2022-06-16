---
layout: default

grand_parent: 3. Extension3 Package
parent: TreeView Class

title: Properties
nav_order: 1
permalink: /package/extension3/treeview/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TreeView class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AcceptDrop](/package/extension3/treeview/properties/acceptdrop) | CRW | integer | 0 | Type that accepts drag and drop <br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[BgColor](/package/extension3/treeview/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/extension3/treeview/properties/border) | CR | boolean | $FALSE | Frame display|
|[Editable](/package/extension3/treeview/properties/editable) | CRW | boolean | $TRUE | Editability|
|[FgColor](/package/extension3/treeview/properties/fgcolor) | CRW | integer | $STD | Text color|
|[FontFace](/package/extension3/treeview/properties/fontface) | CR | integer | $STD |Font decoration attributes |
|[FontKind](/package/extension3/treeview/properties/fontkind) | CR | integer | $STD |Font type <br><small><span style="color:red">Supported fonts have been added since Ver.4.1.0</span></small> |
|[FontSize](/package/extension3/treeview/properties/fontsize) | CR | integer | 10 |Font size |
|[Value](/package/extension3/treeview/properties/value)* | CRW | integer |  |Selected position |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
