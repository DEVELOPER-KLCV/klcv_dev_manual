---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.DisplayOrient Property
nav_order: 24
permalink: /package/standard/root/properties/displayorient
---
# {{ page.title }}
<br>

A property to get or set the direction of screen rotation. The specified value is an absolute value, not a relative value.

Whether the setting is valid and the orientation of the 0 degree state depends on the model.

<u><b> For Mobile Version </b></u>

Specify one of the following values

|   Constant  | Description                    |
|:-----------:|--------------------------------|
|  Root.deg0  | 0 degrees (standard condition) |
|  Root.deg90 | 90 degree rotation             |
| Root.deg180 | 180 degree rotation            |
| Root.deg270 | 270 degree rotation            |

The default value is Root.deg0 .

<u><b> For Android Version </b></u>

Specify one of the following values

|     Constant     | Description                          |
|:----------------:|--------------------------------------|
| Root.UNSPECIFIED | Not in control ( standard condition) |
| Root.LANDSCAPE   | Fix horizontally                     |
| Root.PORTRAIT    | Fix vertically                       |

The default value is Root.UNSPECIFIED .

<br><small><span style="color:red">Can only be used with Mobile, AI</span></small>
<br><small><span style="color:red">Only supported in Mobile Ver.3.1.0 and later version</span></small>