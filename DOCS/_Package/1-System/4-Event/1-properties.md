---
layout: default

grand_parent: 1. System Package
parent: Event Class

title: Properties
nav_order: 1
permalink: /package/system/event/properties

---
# {{ page.title }}


The following properties are defined in the Event class.

|Name       | Access | Type   | Description |
|----------	|--------|--------|-------------|
| [EventName](/package/system/event/properties/EventName) 	| CR 	 |String  |Event name|
| [From](/package/system/event/properties/From) 	| R 	 |reference  |Event source|
| [Reason](/package/system/event/properties/Reason)* 	| CR 	 |integer  |Event type|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property