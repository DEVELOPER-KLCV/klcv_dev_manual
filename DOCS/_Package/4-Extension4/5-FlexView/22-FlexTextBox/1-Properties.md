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
|[AutoCursorMove](/package/extension4/flexview/flextextbox/properties/autocursormove) | CR | boolean |  $FALSE | Automatic movement of cell cursor<br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[Border](/package/extension4/flexview/flextextbox/properties/border) | CRW | boolean |  $FALSE | Display frame  |
|[BorderStyle](/package/extension4/flexview/flextextbox/properties/borderstyle) | CRW | integer |  $SUNKEN | Border style |
|[Copyable](/package/extension4/flexview/flextextbox/properties/copyable) | CRW | boolean|  | Copyability <br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |   
|[Editable](/package/extension4/flexview/flextextbox/properties/editable) | CRW | boolean | $TRUE  | Editability   |
|[IMEMode](/package/extension4/flexview/flextextbox/properties/imemode) | CR | integer|  | IME control <br><small><span style="color:blue">There's a limit in AI</span></small> |
|[InputMode](/package/extension4/flexview/flextextbox/properties/inputmode) | CR | integer|  | Specifying the type of characters that can be entered <br><small><span style="color:green">Specifiable values have been added since Ver.5.0.3.</span></small>  |
|[MaxLength](/package/extension4/flexview/flextextbox/properties/maxlength) | CR | integer|  | Maximum number of bytes that can be entered   <br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[Value](/package/extension4/flexview/flextextbox/properties/value)* | CRW | | String<br>Number<br>Fixed<br>Date<br>UString | Initial value of cell   <br><small><span style="color:green">Added UString since Ver.5.0.0</span></small> | 

Only for both Mobile and Android version

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[UseTapAndHold](/package/extension4/flexview/flextextbox/properties/usetapandhold) | CRW | boolean |  $FALSE |Whether to use tap and hold operation <br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small>  |

Only for both Mobile version

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[DisableEditKey](/package/extension4/flexview/flextextbox/properties/disableeditkey) | CRW | boolean |  $FALSE | Controls the operation to switch to edit mode by pressing the F2 key <br><small><span style="color:red">Added since Mobile Ver.4.5.2</span></small>  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property