---
layout: default

grand_parent: 2. Standard Package
parent: TextBox Class

title: Properties
nav_order: 1
permalink: /package/standard/textbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TextBox class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoComplete](/package/standard/textbox/properties/autocomplete) | CRW | boolean | $FALSE |Whether to perform auto-completion <br><small><span style="color:red">Added since AI Ver.5.0.0</span></small><br><small><span style="color:blue">Connot be used in Mobile, AI</span></small> |
|[AutoTab](/package/standard/textbox/properties/autotab) | CRW | boolean | $FALSE | Automatically move focus by entering all digits|
|[Border](/package/standard/textbox/properties/border) | CR | boolean | $TRUE |Frame display |
|[Format](/package/standard/textbox/properties/format) | CR | String |  |Format string <br><small><span style="color:green">Formats that can be specified from Ver3 have been added have been added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>|
|[HorizontalAlign](/package/standard/textbox/properties/horizontalalign) | CR | integer | $STD | Horizontal alignment<br><small><span style="color:blue">Connot be used in Mobile, AI</span></small>|
|[InputMode](/package/standard/textbox/properties/inputmode) | CR | integer |  |Specifying character types that can be entered <br><small><span style="color:green">Specifiable values have been added since Ver.5.0.3</span></small> |
|[MaxLength](/package/standard/textbox/properties/maxlength) | CR | integer |  | Number of character bytes that can be entered (number of characters in Mobile version and Android version)|
|[Password](/package/standard/textbox/properties/password) | CR | boolean | $FALSE | Input character mask by＊ |
|[Value](/package/standard/textbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | Value to display in the text box<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|
|[VerticalAlign](/package/standard/textbox/properties/verticalalign) | CR | integer | $STD |Vertical alignment (only when printing)<br><small><span style="color:blue">Connot be used in Mobile, AI</span></small> |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable
