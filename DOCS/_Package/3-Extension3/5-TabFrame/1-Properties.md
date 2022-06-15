---
layout: default

grand_parent: 3. Extension3 Package
parent: TabFrame Class

title: Properties
nav_order: 1
permalink: /package/extension3/tabframe/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TabFrame class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[Arrangement](/package/extension3/tabframe/properties/arrangement) | CR | integer | $STD | How to arrange tabs<br><small><span style="color:blue">There's a limit in AI</span></small> |
|[BgColor](/package/extension3/tabframe/properties/bgcolor) | CRW | integer | $STD |Background color |
|[Border](/package/extension3/tabframe/properties/border) | CR | boolean | $FALSE | Display frame|
|[FontFace](/package/extension3/tabframe/properties/fontface) | CR | integer | $STD |Font decoration attributes<br><small><span style="color:blue">There's a limit in AI</span></small> |
|[FontKind](/package/extension3/tabframe/properties/fontkind) | CR | integer | $STD | Font type<br><small><span style="color:red">Supported fonts have been added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><small><span style="color:blue">There's a limit in AI</span></small>|
|[FontSize](/package/extension3/tabframe/properties/fontsize) | CR | integer | 10 | Font size|
|[TabHeight](/package/extension3/tabframe/properties/tabheight) | CRW | integer |  |Tab height |
|[TabPosition](/package/extension3/tabframe/properties/tabposition) | CR | integer | $STD |Tab position<br><small><span style="color:blue">There's a limit in AI</span></small> |
|[TabStyle](/package/extension3/tabframe/properties/tabstyle) | CR | integer | $STD | Tab style <br><small><span style="color:blue">There's a limit in AI</span></small>|
|[TabWidth](/package/extension3/tabframe/properties/tabwidth) | CRW | integer |  | Tab width|
|[Value](/package/extension3/tabframe/properties/value)* | CRW | integer |  |Selected position |

Only for Mobile, Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[UseTapAndHold](/package/extension3/tabframe/properties/usetapandhold) | CRW | boolean | $FALSE | Whether to use tap and hold operation<br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
