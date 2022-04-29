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
|[AcceptDrop](/package/extension5/stree/properties/acceptdrop) | CRW | integer | 0 | |
|[BgColor](/package/extension5/stree/properties/bgcolor) | CRW | integer | $STD | |
|[Border](/package/extension5/stree/properties/border) | CR | boolean | $FALSE | |
|[Editable](/package/extension5/stree/properties/editable) | CR | boolean | $FALSE | |
|[FgColor](/package/extension5/stree/properties/fgcolor) | CRW | integer | $STD | |
|[FirstVisibleItem](/package/extension5/stree/properties/firstvisibleitem) | R | STreeItem |  | |
|[FontFace](/package/extension5/stree/properties/fontface) | CR | integer | $STD | |
|[FontKind](/package/extension5/stree/properties/fontkind) | CR | integer | $STD | |
|[FontSize](/package/extension5/stree/properties/fontsize) | CR | integer | 10 | |
|[LastVisibleItem](/package/extension5/stree/properties/lastvisibleitem) | R | STreeItem |  | |
|[RootItem](/package/extension5/stree/properties/rootitem) | R | STreeItem |  | |
|[SelectedItem](/package/extension5/stree/properties/selecteditem) | R | STreeItem |  | |
|[ToolTip](/package/extension5/stree/properties/tooltip) | CRW | String |  | |
|[ToolTipDelayTime](/package/extension5/stree/properties/tooltipdelaytime) | CRW | integer | 0 | |
|[ToolTipDelayTime](/package/extension5/stree/properties/tooltipdelaytime) | CRW | integer | 0 | |
|[Value](/package/extension5/stree/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property