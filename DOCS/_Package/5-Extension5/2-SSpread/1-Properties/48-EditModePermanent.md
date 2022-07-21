---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.EditModePermanent Property
nav_order: 48
permalink: /package/extension5/sspread/properties/editmodepermanent
---
# {{ page.title }}


Set whether to keep the input mode always ON.

Specify the following values. The initial value is $FALSE.

| Constant | Description                                                |
|----------|------------------------------------------------------------|
| $TRUE    | Always turn on input mode even if you move the active cell |
| $FALSE   | Turn off the input mode                                    |

If you set $TRUE to move the active cell, the <a href="/package/extension5/sspread/event/editmodeoff">EditModeOff</a> event will be fired in the cell before the move and the <a href="/package/extension5/sspread/event/editmodeon">EditModeOn</a> event will be fired in the cell after the move.

Related Item<br>
<a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a>, <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a> event