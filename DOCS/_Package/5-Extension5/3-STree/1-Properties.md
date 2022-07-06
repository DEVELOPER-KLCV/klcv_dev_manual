---
layout: default

grand_parent: 5. Extension5 Package
parent: STree Class

title: Properties
nav_order: 1
permalink: /package/extension5/stree/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the STree class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|----------|
|[AcceptDrop](/package/extension5/stree/properties/acceptdrop) | CRW | integer | 0 |Type that accepts drag and drop |
|[BgColor](/package/extension5/stree/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/extension5/stree/properties/border) | CR | boolean | $FALSE | Display frame|
|[Editable](/package/extension5/stree/properties/editable) | CR | boolean | $FALSE |Editability |
|[FgColor](/package/extension5/stree/properties/fgcolor) | CRW | integer | $STD |Text color |
|[FirstVisibleItem](/package/extension5/stree/properties/firstvisibleitem) | R | STreeItem |  | Accessor for the first displayed item|
|[FontFace](/package/extension5/stree/properties/fontface) | CR | integer | $STD |Font decoration attributes |
|[FontKind](/package/extension5/stree/properties/fontkind) | CR | integer | $STD |Font type |
|[FontSize](/package/extension5/stree/properties/fontsize) | CR | integer | 10 |Font size |
|[LastVisibleItem](/package/extension5/stree/properties/lastvisibleitem) | R | STreeItem |  | Accessor for the last displayed item|
|[RootItem](/package/extension5/stree/properties/rootitem) | R | STreeItem |  | Root item accessor|
|[SelectedItem](/package/extension5/stree/properties/selecteditem) | R | STreeItem |  |Accessor for the selected item |
|[ToolTip](/package/extension5/stree/properties/tooltip) | CRW | String |  | Tooltip|
|[ToolTipDelayTime](/package/extension5/stree/properties/tooltipdelaytime) | CRW | integer | 0 |Tooltip display time |
|[Value](/package/extension5/stree/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property