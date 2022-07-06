---
layout: default

grand_parent: 5. Extension5 Package
parent: HtmlView Class

title: Properties
nav_order: 1
permalink: /package/extension5/htmlview/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the HtmlView class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[AcceptDrop](/package/extension5/htmlview/properties/acceptdrop) | CR | integer | 0 | Specifies the type that accepts drag and drop|
|[AllowAction](/package/extension5/htmlview/properties/allowaction) | CRW | integer | 0 | Specifies the actions to allow<br><small><span style="color:green">Specifiable values have been added from Ver.5.0.3</span></small>|
|[Border](/package/extension5/htmlview/properties/border) | CR | boolean | $FALSE | Specifies the display of the frame|
|[Scroll](/package/extension5/htmlview/properties/scroll) | CR | integer | $AUTO | Display control of the scroll bar. $STATIC is considered the same as $AUTO.<br><small><span style="color:red">Added since Ver.5.0.3</span></small>|
|[Silent](/package/extension5/htmlview/properties/silent) | CR | boolean | $TRUE |Specifies to suppress the warning dialog output from HtmlView<br><small><span style="color:red">Added since Ver.5.0.4</span></small> |
|[URL](/package/extension5/htmlview/properties/url) | R | String |  |The URL of the displayed page |
|[Value](/package/extension5/htmlview/properties/value)* | CRW | String<br>UString |  |Get the HTML of the displayed page or set the HTML to be displayed |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property