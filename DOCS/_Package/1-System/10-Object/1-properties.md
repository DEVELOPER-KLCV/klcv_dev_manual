---
layout: default

grand_parent: 1. System Package
parent: Object Class

title: Properties
nav_order: 1
permalink: /package/system/object/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Object class.

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
| [ClassName](/package/system/object/properties/classname) 	| R | String |Class name <br><small>Added since Version 4.0.0, Mobile Version 3.0.0</small> |
| [IsArray](/package/system/object/properties/isarray) 	| R | boolean | Whether the object is an array<br><small>Added since Version 5.0.0, Mobile Version 1.0.1<br>Not supported on mobile</small>   |
| [Name](/package/system/object/properties/name) 	| R | String | Object name  |
| [ValueType](/package/system/object/properties/valuetype) 	| - | - |  Object data type  |

Properties added only to array objects

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
| [Index](/package/system/object/properties/_index) 	| R | integer |Position of array elements  |
| [Length](/package/system/object/properties/length) 	| R | integer |Number of elements in an array object

  |

Mobile version only

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
| [Class](/package/system/object/properties/class) 	| R | integer |Same as ClassName<br><small>Only Mobile is supported for compatibility</small>  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable