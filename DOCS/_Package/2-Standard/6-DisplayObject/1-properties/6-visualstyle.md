---
layout: default

grand_parent: DisplayObject Class
parent: Properties
has_children: false
title: DisplayObject.VisualStyle property
nav_order: 6
permalink: /package/standard/displayobject/properties/visualstyle
---
# {{ page.title }}

Specifying $ TRUE enables the Windows visual style.

Specifying $ FALSE disables Windows visual styles.

When visual styles are enabled, the Luna style is applied for Windows XP and the Aero style is applied for Windows Vista and Windows 7. It has a visual effect, but it takes a little more processing time.

Disable visual styles if you prioritize performance, and enable visual styles if you prioritize visual effects.

Not all DisplayObject-derived classes support visual-styled display. In addition, since the visual style gives priority to the sense of unity with the OS, the color specification unique to each class may be invalid. See the description of each class for details.

<small>Added since Ver.5.0.0 <br> Not supported in Mobile, AI</small>