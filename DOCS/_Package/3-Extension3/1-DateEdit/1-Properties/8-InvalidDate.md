---
layout: default

grand_parent: DateEdit Class
parent: Properties
has_children: false
title: DateEdit.InvalidDate Property
nav_order: 8
permalink: /package/extension3/dateedit/properties/invaliddate
---
# {{ page.title }}
<br>

If the date entered from the screen is incorrect, it will be $TRUE. If the date is correct or not entered, it will be $FALSE.

By checking this property and the Value property, you can see what kind of input was made.

| Value             |  Invalid Date | Description                   |
|-------------------|---------------|-------------------------------|
| Greater than 0    | $FALSE        | The date is entered correctly |
| Greater than 0    | $TRUE         | Incorrect date entered        |
| 0                 | $FALSE        | Nothing has been entered      |
| 0                 | $TRUE         | Incorrect date entered        |

This property is set by the value entered on the screen when it is confirmed.

It is not set when the Value property is rewritten from the script.