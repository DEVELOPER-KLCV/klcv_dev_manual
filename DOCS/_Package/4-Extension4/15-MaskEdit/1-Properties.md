---
layout: default

grand_parent: 4. Extension4 Package
parent: MaskEdit Class

title: Properties
nav_order: 1
permalink: /package/extension4/maskedit/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the MaskEdit class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[AutoTab](/package/extension4/maskedit/properties/autotab) | CRW | boolean |  | Automatically move focus by entering all digits|
|[Border](/package/extension4/maskedit/properties/border) | CR | boolean | $TRUE | Frame display|
|[EditText](/package/extension4/maskedit/properties/edittext) | R | String |  |The character string displayed on the screen|
|[HorizontalAlign](/package/extension4/maskedit/properties/horizontalalign) | CR | integer | $STD |Horizontal alignment |
|[InputMode](/package/extension4/maskedit/properties/inputmode) | CR | integer |  |Specifying character types that can be entered<br><small><span style="color:green">Specifiable values have been added since Ver.5.0.3</span></small> |
|[InvalidText](/package/extension4/maskedit/properties/invalidtext) | R | boolean | $FALSE | Existence of invalid input|
|[Mask](/package/extension4/maskedit/properties/mask) | CRW※ | String |  | Mask string|
|[UndecidedColor](/package/extension4/maskedit/properties/undecidedcolor) | CR | integer |  | Display format for incorrect input|
|[Value](/package/extension4/maskedit/properties/value)* | CRW | String |  | Value to be displayed in mask edit|
|[VerticalAlign](/package/extension4/maskedit/properties/verticalalign) | CR | integer | $STD |Vertical alignment (only when printing)<br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |

※The Mobile version is CR.

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property