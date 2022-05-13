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
|[AcceptDrop](/package/standard/label/properties/acceptdrop) | CRW | integer | 0  |             |
|[BgColor](/package/standard/label/properties/bgcolor) | CRW | integer | $STD  |             |
|[Border](/package/standard/label/properties/border) | CRW | boelean | $FALSE  |             |
|[BorderStyle](/package/standard/label/properties/borderstyle) | CRW | integer | $SUNKEN  |             |
|[FgColor](/package/standard/label/properties/fgcolor) | CRW | integer | $STD  |             |
|[FontFace](/package/standard/label/properties/fontface) | CR | integer | $STD  |             |
|[FontKind](/package/standard/label/properties/fontkind) | CR | integer | $STD  |             |
|[FontSize](/package/standard/label/properties/fontsize) | CR | integer | 10  |             |
|[Format](/package/standard/label/properties/format) | CR | String |   |             |
|[HorizontalAlign](/package/standard/label/properties/horizontalalign) | CR | integer | $STD  |             |
|[NoPrefix](/package/standard/label/properties/noprefix) | CRW | boolean | $FALSE  |             |
|[ToolTip](/package/standard/label/properties/tooltip) | CRW | String |   |             |
|[ToolTipDelayTime](/package/standard/label/properties/tooltipdelaytime) | CRW | integer | 0  |             |
|[Transparent](/package/standard/label/properties/transparent) | CRW | boolean | $FALSE  |             |
|[Value](/package/standard/label/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |   |             |
|[VerticalAlign](/package/standard/label/properties/verticalalign) | CR | integer | $STD  |             |
|[WordWrap](/package/standard/label/properties/wordwrap) | CRW | boolean | $TRUE  |             |

Only available for Mobile, Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[UseTapAndHold](/package/standard/label/properties/usetapandhold) | CRW | boolean | $FALSE  |             |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
