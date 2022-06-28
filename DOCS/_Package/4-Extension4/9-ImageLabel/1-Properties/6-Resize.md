---
layout: default

grand_parent: ImageLabel Class
parent: Properties
has_children: false
title: ImageLabel.Resize Property
nav_order: 6
permalink: /package/extension4/imagelabel/properties/resize
---
# {{ page.title }}

Specifies how to enlarge/ reduce the image.

| Constant   | Value | Description                                                     |
|------------|:-----:|-----------------------------------------------------------------|
| $STD       |   0   | Original image size (no enlargement/ reduction)                 |
| $KEEPRATIO |   1   | Enlarge/ reduce to the specified size with a fixed aspect ratio |
| $FREE      |   2   | Enlarge/ reduce to the specified size                           |

Enlargement/ reduction is performed based on the values specified in the <a href="/package/extension4/imagelabel/properties/imagewidth">ImageWidth</a> and <a href="/package/extension4/imagelabel/properties/imageheight">ImageHeight</a> properties.