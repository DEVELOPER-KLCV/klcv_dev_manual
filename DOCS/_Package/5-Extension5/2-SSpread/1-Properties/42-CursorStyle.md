---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CursorStyle Property
nav_order: 42
permalink: /package/extension5/sspread/properties/cursorstyle
---
# {{ page.title }}

Sets the shape of the mouse cursor to be used.

Specify the following values. The initial value is $CursorStyleDefault.

| Constant                 | Value | Description                                                 |
|--------------------------|:-----:|-------------------------------------------------------------|
| $CursorStyleUserDefined  |   0   | User-defined icon (cursor specified by CursorIcon property) |
| $CursorStyleDefault      |   1   | Spreadsheet standard cursor (cross-shaped cursor)           |
| $CursorStyleArrow        |   2   | Windows standard arrow cursor                               |
| $CursorStyleDefColResize |   3   | Standard column resizing cursor                             |
| $CursorStyleDefRowResize |   4   | Standard row resizing cursor                                |


Before setting this property, set the <a href="/package/extension5/sspread/properties/cursortype">CursorType</a>  property to select what you want to change the mouse cursor to.

To specify $CursorStyleUserDefined (user-defined), first specify the cursor file with the <a href="/package/extension5/sspread/properties/cursoricon">CursorIcon</a> property.

If the <a href="/package/extension5/sspread/methods/displayobjectsetcursor">DisplayObject.SetCursor</a> method sets a mouse cursor on the entire SSpread object or the parent Form object, that mouse cursor takes precedence and the cursor set with this property is temporarily disabled. If it is canceled by the <a href="/package/extension5/sspread/methods/displayobjectresetcursor">DisplayObject.ResetCursor</a> method, it returns to the cursor set by this property.

Example of usage<br>
```
CursorType = $ CursorTypeDefault;
CursorStyle = $ CursorStyleArrow;
 
CursorIcon = "lock.ani";
CursorType = $ CursorTypeLockedCell;
CursorStyle = $ CursorStyleUserDefined;
```

Related items <br>
<a href="/package/extension5/sspread/properties/cursoricon">CursorIcon</a>, <a href="/package/extension5/sspread/properties/cursortype">CursorType</a> property <br>
<a href="/package/extension5/sspread/methods/displayobjectsetcursor">DisplayObject.SetCursor</a>, <a href="/package/extension5/sspread/methods/displayobjectresetcursor">DisplayObject.ResetCursor</a> method
