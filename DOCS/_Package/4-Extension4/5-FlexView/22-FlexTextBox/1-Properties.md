---
layout: default

grand_parent: FlexView Class
parent: FlexTextBox Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flextextbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexTextBox class.

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[AutoCursorMove](/package/extension4/flexview/flextextbox/properties/autocursormove) | CR | boolean |  $FALSE |
|[Border](/package/extension4/flexview/flextextbox/properties/border) | CRW | boolean |  $FALSE |
|[BorderStyle](/package/extension4/flexview/flextextbox/properties/borderstyle) | CRW | integer |  $SUNKEN |
|[Copyable](/package/extension4/flexview/flextextbox/properties/copyable) | CRW | boolean |   |
|[Editable](/package/extension4/flexview/flextextbox/properties/editable) | CRW | boolean | $TRUE  |
|[IMEMode](/package/extension4/flexview/flextextbox/properties/imemode) | CR | integer |   |
|[InputMode](/package/extension4/flexview/flextextbox/properties/inputmode) | CR | integer |   |
|[MaxLength](/package/extension4/flexview/flextextbox/properties/maxlength) | CR | integer |   |
|[Value](/package/extension4/flexview/flextextbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |   |

Only for both Mobile and Android version

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[UseTapAndHold](/package/extension4/flexview/flextextbox/properties/usetapandhold) | CRW | boolean |  $FALSE |

Only for both Mobile version

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[DisableEditKey](/package/extension4/flexview/flextextbox/properties/disableeditkey) | CRW | boolean |  $FALSE |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property