---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AllowDragDrop Property
nav_order: 7
permalink: /package/extension5/sspread/properties/allowdragdrop
---
# {{ page.title }}

Set whether to allow the user to move or copy cell blocks by dragging and dropping.

Specify $TRUE to allow it, or $FALSE to disallow it.

The initial value is $FALSE.

If allowed, the cell block can be moved by dragging the edge of the selected cell block. Hold down the Ctrl key while dragging to copy the cell block.

Dragging and dropping a cell block raises the <a href="/package/extension5/sspread/events/dragdropblock">DragDropBlock</a> event.

The mouse cursor associated with drag and drop can be changed with the <a href="/package/extension5/sspread/properties/cursoricon">CursorIcon</a>, <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a>, and <a href="/package/extension5/sspread/properties/cursortype">CursorType</a> properties.

Related Item <br>
<a href="/package/extension5/sspread/properties/cursoricon">CursorIcon</a>, <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a>, <a href="/package/extension5/sspread/properties/cursortype">CursorType</a> property<br>
<a href="/package/extension5/sspread/events/dragdropblock">DragDropBlock</a> event