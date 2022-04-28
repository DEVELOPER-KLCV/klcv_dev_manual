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
|[AutoTab](/package/extension4/maskedit/properties/autotab) | CRW | boolean |  | |
|[Border](/package/extension4/maskedit/properties/border) | CR | boolean | $TRUE | |
|[EditText](/package/extension4/maskedit/properties/edittext) | R | String |  | |
|[HorizontalAlign](/package/extension4/maskedit/properties/horizontalalign) | CR | integer | $STD | |
|[InputMode](/package/extension4/maskedit/properties/inputmode) | CR | integer |  | |
|[InvalidText](/package/extension4/maskedit/properties/invalidtext) | R | boolean | $FALSE | |
|[Mask](/package/extension4/maskedit/properties/mask) | CRW※ | String |  | |
|[UndecidedColor](/package/extension4/maskedit/properties/undecidedcolor) | CR | integer |  | |
|[Value](/package/extension4/maskedit/properties/value)* | CRW | String |  | |
|[VerticalAlign](/package/extension4/maskedit/properties/verticalalign) | CR | integer | $STD | |

※The Mobile version is CR.

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property