---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetFontFamily Property
nav_order: 21
permalink: /package/standard/root/methods/setfontfamily
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add available fonts.<br>Specifies the font that corresponds to the <a href="/base/fontkind">FontKind</a> property setting defined for each class.<br><br>In the initial state, "MS Gothic" and "MS P Gothic" are set in $ STD, and "MS Mincho" and "MS P Mincho" are set in $ FONT1. If you want to use a font other than these, you can assign any font to the setting value of the FontKind property with the SetFontFamily method.<br><br>Displaying with the assigned font is valid only for the FontKind property that is set after executing the SetFontFamily method. The already displayed font cannot be changed with the SetFontFamily method.<br><br>Normally, call the SetFontFamily method before displaying the screen when the application is initialized. <br>Also, the FontKind properties $ STD and $ FONT1 are used by the system and should not be changed.<br><br>The font allocation returns to the initial state when the <a href="/package/standard/root/methods/login">Login</a> and <a href="/package/standard/root/methods/logout">Logout</a> methods are executed.<br><br>Be sure to specify the font installed on your computer for <b><i>p_font></i></b> and <b><i>c_font</i></b>. If you specify a font that does not exist on your computer, the display result is undefined. In addition, the display result of characters that the font does not have (for example, when Japanese is displayed with the alphabetic font "Arial") is also undefined.<br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><br><small><span style="color:red">The following specifications have been added in ver4.1.3.4 or later.</span></small><br>For the font name specified in <b><i>p_font></i></b> and <b><i>c_font</i></b>, you can specify the adjustment value of the character size when actually using it in the following format.
    <code><pre>fontname/ratio</pre></code><br>Specify the font name in fontname and the magnification of the font size in ratio. If the ratio is a positive number, it is based on the cell size, and if it is a negative number, it is based on the glyph size.<br> Example<br>"Merio"     It is the same specification as before. Font size is based on cell size. <br>"Merio / 120"     It is 120% of the size based on the cell size.<br> "Merio / -100"    It will be 100% based on the glyph size.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetFontFamily( <b>kind</b>, <b>p_font</b> [, <b>c_font</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>kind</b></td>
    <td>Setting value of FontKind property to assign font<br>Specify $ FONT2 to $ FONT7</td>
  </tr>
  <tr>
    <td>String <b>p_font</b></td>
    <td>Specify the font name used in the proportional display.</td>
  </tr>
  <tr>
    <td>String <b>c_font</b></td>
    <td>Specifies the font used for fixed pitch display. If this parameter is omitted, the same font as p_font will be used for fixed pitch display.<br><br>If you specify the $ FIXED attribute for the FontFace property, it will be displayed in the font specified here, but it will be displayed at a fixed pitch only when the specified font is defined as a fixed pitch. If the font is defined with a variable pitch, it may be displayed with a variable pitch even if the $ FIXED attribute is specified.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>PKG-59</td>
    <td>FontKind argument is invalid</td>
  </tr>
  <tr>
    <td>PKG-59</td>
    <td>FontName argument is invalid</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetFontFamily($FONT2, "Arial");
 
Label b {
    :
    FontKind = $FONT2;
    Value = "Arial Font";
    :
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/getfontfamily">GetFontFamily</a> method</td>
  </tr>
</table>



