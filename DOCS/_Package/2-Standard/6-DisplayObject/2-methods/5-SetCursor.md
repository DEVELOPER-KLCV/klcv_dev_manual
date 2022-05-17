---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.SetCursor Method
nav_order: 5
permalink: /package/standard/displayobject/methods/setcursor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the mouse cursor.<br><br>The mouse cursor that can be specified with the SetCursor method is standard Windows mouse pointer data with a .cur or .ani extension.<br>Since the mouse cursor is changed immediately by calling the method, it is possible to change the mouse cursor before the time-consuming process and return it after the process is completed.<br><br>In an object tree starting with "//" (<a href="/package/standard/root/">Root</a> object), if the mouse cursor is set in multiple hierarchies with the SetCursor method, the higher setting takes precedence. For example, if you execute the SetCursor method on both a Form object and a Button object placed as a child of it, the specified cursor will be displayed on the Form object even if the mouse cursor moves over the Button object.<br><br>Call the <a href="/package/standard/displayobject/methods/resetcursor">ResetCursor</a> method to return the set mouse cursor to standard.<br><br>Mouse cursors may have restrictions on the formats available depending on the display hardware. For example, one display can only use a monochrome two-tone mouse cursor. For applications that may run on older computers, make sure to use the mouse cursor in a format that is available on the intended computer.<br><br><b>Mobile version</b><br>Shows the weight cursor. It takes an argument to maintain compatibility with the PC version, but the argument is not used.<br><br>Also, unlike the PC version, each object is not distinguished. Calling this method from any object will have similar results.<br><br>To stop displaying the wait cursor, call the ResetCursor method.<br><br><b>Android version</b><br>Display the wait dialog. The wait dialog is always displayed in the center of the screen and you cannot perform any other operations while it is displayed.<br><br>Also, as with the Mobile version, no distinction is made for each object. Calling this method from any object will have similar results.<br><br>To stop displaying the wait dialog, call the ResetCursor method.<br><br><small><p style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0, AI Ver.1.0.1</p></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2"><b>PC, Mobile version</b><br>
obj.SetCursor( <b>URL or reader</b> )<br>
<b>Android version</b><br>obj.SetCursor( [ <b>message</b> [, <b>title</b> ]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>URL or reader</b></td>
    <td>Specify the URL or <a href="/base/readerwriter#reader-object"> Reader object</a> to get the cursor data.<br><br>When specifying the URL, you can specify it with a relative path or an absolute path, and the cursor data is downloaded and displayed.<br>Only when the URL is specified, it will be cached.<br><br><b>Mobile version</b><br>Any value</td>
  </tr>
  <tr>
    <td>String <b>message</b></td>
    <td>Specify the character string of the message part of the wait dialog.<br>If omitted, "Please wait" is displayed.<br>If an empty string is specified, no message is displayed.</td>
  </tr>
  <tr>
    <td>String <b>title</b></td>
    <td>The character string in the title part of the weight dialog.<br>If omitted, "Processing" is displayed.<br>If an empty string is specified, the title will not be displayed.</td>
  </tr>
  <tr>
    <td rowspan="5">Exception</td>
    <td>PKG-57</td>
    <td>Cannot setCursor or ResetCursor on array definition</td>
  </tr>
  <tr>
    <td>PKG-58</td>
    <td>Unable to get cursor data</td>
  </tr>
  <tr>
    <td>PKG-59</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>PKG-60</td>
    <td>Unable to create temporary file</td>
  </tr>
  <tr>
    <td>PKG-61</td>
    <td>Invalid cursor data</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
Function OnTouch(e) {
    //.SetCursor("wait.cur");
    :
    //.ResetCursor();
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/displayobject/methods/resetcursor">ResetCursor</a> method</td>
  </tr>
</table>

