---
layout: default

grand_parent: 2. Standard Package
parent: Label Class

title: Properties
nav_order: 1
permalink: /package/standard/label/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Label class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AcceptDrop](/package/standard/label/properties/acceptDrop) | CRW | integer | 0  |             |
|[BgColor](/package/standard/label/properties/BgColor) | CRW | integer | $STD  |             |
|[Border](/package/standard/label/properties/Border) | CRW | boelean | $FALSE  |             |
|[BorderStyle](/package/standard/label/properties/BorderStyle) | CRW | integer | $SUNKEN  |             |
|[FgColor](/package/standard/label/properties/FgColor) | CRW | integer | $STD  |             |
|[FontFace](/package/standard/label/properties/FontFace) | CR | integer | $STD  |             |
|[FontKind](/package/standard/label/properties/FontKind) | CR | integer | $STD  |             |
|[FontSize](/package/standard/label/properties/FontSize) | CR | integer | 10  |             |
|[Format](/package/standard/label/properties/Format) | CR | String |   |             |
|[HorizontalAlign](/package/standard/label/properties/HorizontalAlign) | CR | integer | $STD  |             |
|[NoPrefix](/package/standard/label/properties/NoPrefix) | CRW | boolean | $FALSE  |             |
|[ToolTip](/package/standard/label/properties/ToolTip) | CRW | String |   |             |
|[ToolTipDelayTime](/package/standard/label/properties/ToolTipDelayTime) | CRW | integer | 0  |             |
|[Transparent](/package/standard/label/properties/Transparent) | CRW | boolean | $FALSE  |             |
|[Transparent](/package/standard/label/properties/Transparent) | CRW | boolean | $FALSE  |             |
|[Value](/package/standard/label/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |   |             |
|[VerticalAlign](/package/standard/label/properties/verticalAlign) | CR | integer | $STD  |             |
|[WordWrap](/package/standard/label/properties/WordWrap) | CRW | boolean | $TRUE  |             |

Only available for Mobile, Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[UseTapAndHold](/package/standard/label/properties/useTapAndHold) | CRW | boolean | $FALSE  |             |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
