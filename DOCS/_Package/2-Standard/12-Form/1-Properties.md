---
layout: default

grand_parent: 2. Standard Package
parent: Form Class

title: Properties
nav_order: 1
permalink: /package/standard/form/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Form class.

|Name       | Access | Type   |  Initial Value | Description  |
|----------	|--------|--------|----------------|--------------|
|[AcceptDrop](/package/standard/form/properties/acceptdrop) | CRW | integer | 0  | |
|[BgColor](/package/standard/form/properties/bgcolor) | CRW | integer | $STD |
|[BgHighQuality](/package/standard/form/properties/bghighquality) | CRW | boolean | $FALSE |
|[BgPattern](/package/standard/form/properties/bgpattern) | CRW | XmlDocument |  |
|[BgPatternCache](/package/standard/form/properties/bgpatterncache) | CRW | boolean | $FALSE |
|[Border](/package/standard/form/properties/border) | CR | boolean | $FALSE |
|[FontScale](/package/standard/form/properties/fontscale) | CRW | Number | 1.0 |
|[HorizontalScale](/package/standard/form/properties/horizontalscale) | CRW | Number | 1.0 |
|[Scroll](/package/standard/form/properties/scroll) | CR | integer | $AUTO |
|[Transparent](/package/standard/form/properties/transparent) | CR | boolean | $FALSE |
|[UseGesture](/package/standard/form/properties/usegesture) | CRW | integer | $STD |
|[UseMouseMove](/package/standard/form/properties/usemousemove) | CRW | integer | $STD |
|[UseMouseWheel](/package/standard/form/properties/usemousewheel) | CRW | integer | $STD |
|[Value](/package/standard/form/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |
|[VerticalScale](/package/standard/form/properties/verticalscale) | CRW | Number | 1.0 |

Only for Mobile, Android version

|Name       | Access | Type   |  Initial Value | Description  |
|----------	|--------|--------|----------------|--------------|
|[usetapandhold](/package/standard/form/properties/UseTapAndHold) | CRW | boolean | $FALSE  | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property