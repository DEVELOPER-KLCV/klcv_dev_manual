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
|[BorderStyle](/package/extension4/groupbox/properties/borderstyle) | CRW | integer | $ETCHED |
|[BoxStyle](/package/extension4/groupbox/properties/boxstyle) | CRW | integer | $BOX |
|[FgColor](/package/extension4/groupbox/properties/fgcolor) | CRW | integer | $STD |
|[FontFace](/package/extension4/groupbox/properties/fontface) | CR | integer | $STD |
|[FontKind](/package/extension4/groupbox/properties/fontkind) | CR | integer | $STD |
|[FontSize](/package/extension4/groupbox/properties/fontsize) | CR | integer | 10 |
|[Title](/package/extension4/groupbox/properties/title) | CRW | String<br>UString(※) |  |
|[TitleAlign](/package/extension4/groupbox/properties/titlealign) | CRW | integer | $LEFT |
|[TitlePosition](/package/extension4/groupbox/properties/titleposition) | CRW | integer | $TOP |
|[Value](/package/extension4/groupbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: Default property