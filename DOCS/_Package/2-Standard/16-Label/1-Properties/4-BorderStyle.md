---
layout: default

grand_parent: Label Class
parent: Properties
has_children: false
title: Label.BorderStyle Property
nav_order: 4
permalink: /package/standard/label/properties/borderstyle
---
# {{ page.title }}

<br>

Specify the border type. Only valid if the <a href="/package/standard/label/properties/border">Border</a> property is $ TRUE .

|   Constant   | Value | Description                                                                                                          |
|:------------:|:-----:|----------------------------------------------------------------------------------------------------------------------|
| $SUNKEN     | 0     | The whole is displayed in a concave shape                                                                            |
| $RISED      | 1     | The whole is displayed in a convex shape                                                                             |
| $ETCHED     | 2     | The line of the frame is displayed in a concave shape.                                                               |
| $BUMP       | 3     | Displays the frame line in a convex shape                                                                            |
| $GRAYFRAME  | 4     | Shows a border in two colors of gray                                                                                 |
| $SOFT       | 5     | Display the frame in black and white                                                                                 |
| $SOFTETCHED | 6     | The border is displayed in a soft concave shape.                                                                     |
| $SOFTBUMP   | 7     | The border is displayed in a soft convex shape.                                                                      |
| $PLANE      | 8     | Display with a single black line                                                                                     |
| $DASH       | 9     | Display with a long dotted line <br><span style="color:blue">On mobile, it will be displayed the same as $DOT</span> |
| $ DOT        | 10    | Display with a fine dotted line                                                                                      |
| $FLATSUNKEN | 11    | Displays the whole with a low concave shape                                                                          |
| $FLATRISED  | 12    | Display the whole with a low convex shape                                                                            |

<small><span style="color:red">Added $PLANE and later version since Ver.4.0.0, Mobile Ver.3.0.0</span></small>


<br>
Display Example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std1p3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<small><span style="color:red">Added since Mobile Ver.2.0.0</span></small>
