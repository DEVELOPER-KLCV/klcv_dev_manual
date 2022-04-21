---
layout: default

grand_parent: 1. System Package
parent: Exception Class

title: Properties
nav_order: 1
permalink: /package/system/exception/properties

---
# {{ page.title }}


The following properties are defined in the Event class.

|Name       | Access | Type   | Description |
|----------	|--------|--------|-------------|
| [Code](/package/system/exception/properties/Code) 	| R 	 |integer  | Exception number|
| [Message](/package/system/exception/properties/Message)* 	| R 	 |String  | Exception description|
| [Method](/package/system/exception/properties/Method) 	| R 	 |String  | The function that caused the exception|
| [SourceOffset](/package/system/exception/properties/SourceOffset) 	| R 	 |integer  | Byte position of the CRS script that raised the exception|
| [SourceURL](/package/system/exception/properties/SourceURL) 	| R 	 |String  | URL of the CRS script that raised the exception|
| [SubCode](/package/system/exception/properties/SubCode) 	| R 	 |Integer  | Auxiliary exception number<br>**<small>Added since Version 5.0.2</small>**<br>**<small>Not compatible with Mobile, AI</small>**|
| [SubMessage](/package/system/exception/properties/SubMessage) 	| R 	 |String  | Auxiliary description<br>**<small>Added since Version 5.0.2</small>**<br>**<small>Not compatible with Mobile, AI</small>**|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property