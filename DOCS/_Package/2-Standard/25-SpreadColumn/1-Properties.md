---
layout: default

grand_parent: 2. Standard Package
parent: SpreadColumn Class

title: Properties
nav_order: 1
permalink: /package/standard/spreadcolumn/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the SpreadColumn class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[BgColor](/package/standard/spreadcolumn/properties/bgcolor) | CRW | integer | $STD |Background color |
|[BreakKey](/package/standard/spreadcolumn/properties/breakkey) | CR | integer |  | Generate key break event|
|[Editable](/package/standard/spreadcolumn/properties/editable) | CRW | boolean | $TRUE | Editability|
|[FgColor](/package/standard/spreadcolumn/properties/fgcolor) | CRW | integer | $STD |Text color |
|[Format](/package/standard/spreadcolumn/properties/format) | CR | String |  |Format string <br><small><span style="color:red">Formats that can be specified have been added since Ver.4.1.0</span></small>|
|[HorizontalAlign](/package/standard/spreadcolumn/properties/horizontalalign) | CR | integer | $STD | Horizontal alignment |
|[Suppress](/package/standard/spreadcolumn/properties/suppress) | CR | integer |  | Do not repeat the same data|
|[Title](/package/standard/spreadcolumn/properties/title) | CRW | String |  | Column header characters|
|[Value](/package/standard/spreadcolumn/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  |Value to display in cell |
|[VerticalAlign](/package/standard/spreadcolumn/properties/verticalalign) | CR | integer | $STD | Vertical alignment|
|[Visible](/package/standard/spreadcolumn/properties/visible) | CRW | boolean | $TRUE | Display control|
|[Width](/package/standard/spreadcolumn/properties/width) | CRW | integer | 100 | Width |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
