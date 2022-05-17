---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.ResetCursor Method
nav_order: 4
permalink: /package/standard/displayobject/methods/resetcursor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the mouse cursor changed by the <a href="/package/standard/displayobject/methods/setcursor">SetCursor</a> method to the standard.<br><br><b>Mobile version , Android version</b><br>Cancels the wait cursor display.<br>Unlike the PC version, it does not distinguish between objects.<br><br><small><p style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0, AI Ver.1.0.1</p></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.ResetCursor( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-57</td>
    <td>Cannot setCursor or ResetCursor on array definition</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
function OnTouch(e) {
    //.SetCursor("wait.cur");
    :
    //.ResetCursor();
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/displayobject/methods/setcursor">SetCursor</a> method</td>
  </tr>
</table>

