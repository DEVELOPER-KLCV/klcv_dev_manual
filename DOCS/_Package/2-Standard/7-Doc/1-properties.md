---
layout: default

grand_parent: 2. Standard Package
parent: Doc Class

title: Properties
nav_order: 1
permalink: /package/standard/doc/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Doc class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[Format](/package/standard/doc/properties/format) | CR | String | "A4V" | Paper size |
|[Height](/package/standard/doc/properties/height) | CRW | integer |  | Paper height  |
|[OverLay](/package/standard/doc/properties/overlay) | CRW | XmlDocument | | SVG to print on the front  |
|[PageNumber](/package/standard/doc/properties/pagenumber) | R | integer |  | Page number |
|[Preview](/package/standard/doc/properties/preview) | CR | integer | $PRINTER | Print destination |
|[Printer](/package/standard/doc/properties/printer) | CR | String |  | Output destination printer name |
|[Title](/package/standard/doc/properties/title) | CR | String |  | Document title |
|[Value](/package/standard/doc/properties/value)* | CR | String<br>Number<br>Fixed<br>Date |  |Object value  |
|[Width](/package/standard/doc/properties/width) | CRW | integer |  | Paper width |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property