---
layout: default

grand_parent: FlexView Class
parent: FlexIndentLabel Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexindentlabel/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexIndentLabel class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[Foldable](/package/extension4/flexview/flexindentlabel/properties/foldable) | CRW | boolean | $TRUE | Propriety of folding | 
|[Folding](/package/extension4/flexview/flexindentlabel/properties/folding) | CRW | boolean | $FALSE | Folded state|
|[Indent](/package/extension4/flexview/flexindentlabel/properties/indent) | CRW | boolean | $TRUE |Indented state<br><small><span style="color:red">Added since Ver.4.1.3</span></small> |
|[Key](/package/extension4/flexview/flexindentlabel/properties/key) | CRW | String |  | Own key|
|[ParentKey](/package/extension4/flexview/flexindentlabel/properties/parentkey) | CRW | String |  | Parent's key|
|[Value](/package/extension4/flexview/flexindentlabel/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | Initial cell value<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property