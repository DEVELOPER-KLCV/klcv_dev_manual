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
| [ClassName](/package/system/object/properties/classname) 	| R | String |  |
| [IsArray](/package/system/object/properties/isarray) 	| R | boolean |  |
| [Name](/package/system/object/properties/name) 	| R | String |  |
| [ValueType](/package/system/object/properties/valuetype) 	| - | - |  |

Properties added only to array objects

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
| [Index](/package/system/object/properties/_index) 	| R | integer |  |
| [Length](/package/system/object/properties/length) 	| R | integer |  |

Mobile version only

|Name       | Access | Type   | Description   |
|----------	|--------|--------|---------------|
| [Class](/package/system/object/properties/class) 	| R | integer |  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable