---
layout: default

grand_parent: 4. Extension4 Package
parent: ListView Class

title: Properties
nav_order: 1
permalink: /package/extension4/listview/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ListView class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[AcceptDrop](/package/extension4/listview/properties/acceptdrop) | CRW | integer | 0 | Type that accepts drag and drop<br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[BgColor](/package/extension4/listview/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/extension4/listview/properties/border) | CR | boolean | $TRUE |Display border |
|[Checkboxes](/package/extension4/listview/properties/checkboxes) | CRW | boolean | $FALSE | Display check boxes|
|[ColFixed](/package/extension4/listview/properties/colfixed) | CRW | boolean | $FALSE | Fixed column|
|[ColHeader](/package/extension4/listview/properties/colheader) | CR | integer | $STD |Column behavior |
|[DragStyle](/package/extension4/listview/properties/dragstyle) | CRW | integer | $STD |Icon behavior |
|[Editable](/package/extension4/listview/properties/editable) | CRW | boolean | $FALSE | Edit text|
|[FgColor](/package/extension4/listview/properties/fgcolor) | CRW | integer | $STD | Text color|
|[FontFace](/package/extension4/listview/properties/fontface) | CR | integer | $STD |Font decoration attributes |
|[FontKind](/package/extension4/listview/properties/fontkind) | CR | integer | $STD |Font type <br><small><span style="color:red">Supported fonts have been added since Ver.4.1.0</span></small>|
|[FontSize](/package/extension4/listview/properties/fontsize) | CR | integer | 10 | Font size|
|[GridLine](/package/extension4/listview/properties/gridline) | CRW | boolean | $FALSE |Display grid lines |
|[HorzIconSpacing](/package/extension4/listview/properties/horziconspacing) | CRW | integer | 46 |Large icon horizontal spacing |
|[ListStyle](/package/extension4/listview/properties/liststyle) | CRW | integer | $LARGEICON | List type|
|[SingleSel](/package/extension4/listview/properties/singlesel) | CR | boolean | $FALSE |Select only one item |
|[TextBgColor](/package/extension4/listview/properties/textbgcolor) | CRW | integer | $STD |Background color in the frame |
|[Value](/package/extension4/listview/properties/value)* | CRW | integer |  | Selected position|
|[VertIconSpacing](/package/extension4/listview/properties/verticonspacing) | CRW | integer | 43 | Large icon vertical spacing|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property