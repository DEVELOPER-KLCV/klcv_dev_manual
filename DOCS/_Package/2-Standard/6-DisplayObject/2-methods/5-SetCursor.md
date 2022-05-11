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
    <td colspan="2"></td>
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
    <td></td>
  </tr>
  <tr>
    <td>String <b>message</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>title</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="5">Exception</td>
    <td>PKG-57</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-58</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-59</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-60</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-61</td>
    <td></td>
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

