---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.GetWrappedString Method
nav_order: 6
permalink: /package/extension4/styleedit/methods/getwrappedstring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns a character string that is broken at the same position as the screen display. The GetWrappedString method can only be called while StyleEdit is initialized and displayed on the screen.<br><br>Also, if Value, Width, WordWrap, WordWrapMode, LineWidthLimit, LineNumber, which affect the line feed position on the display, are changed and GetWrappedString is called before it is reflected in the display, an EXT-20 exception will be thrown. This exception indicates that StyleEdit cannot get the latest line feed position because the screen display determines the line feed position for the first time. However, even in this situation, by specifying true in the force argument, it is possible to forcibly acquire the character string before reflecting the changed property.<br><br>This method always returns a "Word Wrapped String" when run within Biz / Designer.<br><small><span style="color:red">Added since Ver.4.1.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = StyleEdit1.GetWrappedString( [ <b>force</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>force</b></td>
    <td>If true is specified, a character string will be returned even if the latest property settings are not reflected. If force is omitted or false is specified, an EXT-20 exception will be thrown if the latest character string cannot be obtained.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-20</td>
    <td>Adjustment of the line feed position by changing the property is currently pending.</td>
  </tr>
  <tr>
    <td>EXT-21</td>
    <td>Cannot call GetWrappedString on an object that has not been materialized or has already been deleted</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>