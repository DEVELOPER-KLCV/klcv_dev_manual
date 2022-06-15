---
layout: default

grand_parent: 3. Extension3 Package
parent: NumberEdit Class

title: Properties
nav_order: 1
permalink: /package/extension3/numberedit/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the NumberEdit class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoTab](/package/extension3/numberedit/properties/autotab) | CRW | boolean | $FALSE | Automatically move focus by entering all digits|
|[Border](/package/extension3/numberedit/properties/border) | CR | boolean | $TRUE | Display frame|
|[DisableHelper](/package/extension3/numberedit/properties/disablehelper) | CRW | boolean | $FALSE |Disable the simple calculator display<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Cannot be used in Mobile, AI</span></small> |
|[Format](/package/extension3/numberedit/properties/format) | CR | String |  |Format string<br><small><span style="color:red">The specified character "N" has been added since Ver.4.0.3, Mobile Ver.2.0.0</span></small> |
|[HorizontalAlign](/package/extension3/numberedit/properties/horizontalalign) | CR | integer | $STD |Horizontal alignment |
|[IsNull](/package/extension3/numberedit/properties/isnull) | CRW | boolean |  | Determination when Value property is 0<br><small><span style="color:red">Added since Ver.4.0.3, Mobile Ver.2.0.0</span></small>|
|[MaxLength](/package/extension3/numberedit/properties/maxlength) | CR | integer | 15 | Number of character bytes that can be entered (number of characters in Mobile version and Android version)|
|[Value](/package/extension3/numberedit/properties/value)* | CRW | Date |  | The value to display in the NumberEdit object|
|[VerticalAlign](/package/extension3/numberedit/properties/verticalalign) | CR | integer | $STD |Vertical alignment (printing only) <br><small><span style="color:blue">Cannot be used in Mobile, AI</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
