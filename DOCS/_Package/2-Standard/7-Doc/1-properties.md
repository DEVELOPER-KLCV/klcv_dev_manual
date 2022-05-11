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
|[Format](/package/standard/doc/properties/format) | CR | String | "A4V" |  |
|[Height](/package/standard/doc/properties/height) | CRW | integer |  |  |
|[OverLay](/package/standard/doc/properties/overlay) | CRW | XmlDocument |  |  |
|[PageNumber](/package/standard/doc/properties/pagenumber) | R | integer |  |  |
|[Preview](/package/standard/doc/properties/preview) | CR | integer | $PRINTER |  |
|[Printer](/package/standard/doc/properties/printer) | CR | String |  |  |
|[Title](/package/standard/doc/properties/title) | CR | String |  |  |
|[Value](/package/standard/doc/properties/value)* | CR | String<br>Number<br>Fixed<br>Date |  |  |
|[Width](/package/standard/doc/properties/width) | CRW | integer |  |  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property