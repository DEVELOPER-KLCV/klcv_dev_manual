---
layout: default

grand_parent: 4. Extension4 Package
parent: GroupBox Class

title: Properties
nav_order: 1
permalink: /package/extension4/groupbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the GroupBox class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[BorderStyle](/package/extension4/groupbox/properties/borderstyle) | CRW | integer | $ETCHED | Border type |
|[BoxStyle](/package/extension4/groupbox/properties/boxstyle) | CRW | integer | $BOX | Group box type |
|[FgColor](/package/extension4/groupbox/properties/fgcolor) | CRW | integer | $STD | Text color|
|[FontFace](/package/extension4/groupbox/properties/fontface) | CR | integer | $STD | Font decoration attributes <br><small><span style="color:blue">There's a limit in AI</span></small>|
|[FontKind](/package/extension4/groupbox/properties/fontkind) | CR | integer | $STD |Font type <br><small><span style="color:red">Supported fonts have been added since Ver.4.1.0</span></small><br><small><span style="color:blue">There's a limit in AI</span></small> |
|[FontSize](/package/extension4/groupbox/properties/fontsize) | CR | integer | 10 | Font size|
|[Title](/package/extension4/groupbox/properties/title) | CRW | String<br>UString(※) |  | Display title <br>(※)When ValueType is UString <small><span style="color:red">Added since Ver.5.0.3</span></small>|
|[TitleAlign](/package/extension4/groupbox/properties/titlealign) | CRW | integer | $LEFT | Align title string |
|[TitlePosition](/package/extension4/groupbox/properties/titleposition) | CRW | integer | $TOP |Title display position |
|[Value](/package/extension4/groupbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | Object value<br><small><span style="color:red">Added UString since Ver.4.2.0</span></small>| 

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: Default property