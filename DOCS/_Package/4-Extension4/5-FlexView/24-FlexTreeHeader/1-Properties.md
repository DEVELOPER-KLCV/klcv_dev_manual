---
layout: default

grand_parent: FlexView Class
parent: FlexTreeHeader Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flextreeheader/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexTreeHeader class.

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[BgStyle](/package/extension4/flexview/flextreeheader/properties/bgstyle) | CRW | integer |  $INDENT |Background display method|
|[Foldable](/package/extension4/flexview/flextreeheader/properties/foldable) | CRW | boolean |  $TRUE |Propriety of folding operation  |
|[HorizontalAlign](/package/extension4/flexview/flextreeheader/properties/horizontalalign) | CR | integer |  $STD | Horizontal alignment |
|[Value](/package/extension4/flexview/flextreeheader/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString  |  | Initial value of cell<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property