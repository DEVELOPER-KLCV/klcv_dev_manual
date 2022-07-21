---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CursorIcon Property
nav_order: 41
permalink: /package/extension5/sspread/properties/cursoricon
---
# {{ page.title }}

Sets a user-defined mouse cursor. Specify if you want to use any cursor file.

Only valid if the <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a> property is $CursorStyleUserDefined.

Specify the URL string of the cursor file or the <a href="/base/readerwriter#reader-object">Reader Object</a>.

This property is for configuration only. Whenever you get a value, it returns null.

The mouse cursor that can be specified is a standard Windows cursor file with a .cur or .ani extension.

The mouse cursor does not change when this property is set. When $CursorStyleUserDefined is set in the <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a> property, the cursor file set in this property is used.

If you specify a URL, the file will be cached on your local computer for faster loading from the next time onwards.

You can always get the latest files from the server by specifying the <a href="/package/httppackage">HttpResponse</a> object.

Example of usage<br>
```
CursorIcon = "lock.ani";
CursorType = $CursorTypeLockedCell;
CursorStyle = $CursorStyleUserDefined;
 
var fs = new FileSystem;
var fp = fs.Open("cursor\\grayarea.cur", FileSystem.OPEN_READ);
CursorIcon = fp;
fp.Close();
CursorType = $CursorTypeGrayArea;
CursorStyle = $CursorStyleUserDefined;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a>, <a href="/package/extension5/sspread/properties/cursortype">CursorType</a> property <br>
<a href="/package/httppackage">HttpResponse</a> class