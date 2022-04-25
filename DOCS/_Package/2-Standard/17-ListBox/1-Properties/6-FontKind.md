---
layout: default

grand_parent: ListBox Class
parent: Properties
has_children: false
title: FontKind Property
nav_order: 6
permalink: /package/standard/listbox/properties/fontkind
---
# {{ page.title }}


Specify the font type.
 
You can specify $STD and $FONT1 - $FONT7 as the font type.

$STD is a Gothic font, $FONT1 is a Mincho font, and $FONT2 - $FONT7 use the font specified by the [Root.SetFontFamily]() method. The display result is undefined if the font not assigned by the SetFontFamily method in $FONT2 - $FONT7 or the assigned font is not registered in the computer.


<table>
    <tr>
        <td>Constant</td>
        <td>Value</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>$STD</td>
        <td>0</td>
        <td>Gothic</td>
    </tr>
    <tr>
        <td>$FONT1</td>
        <td>1</td>
        <td>Mincho</td>
    </tr>
    <tr>
        <td>$FONT2</td>
        <td>2</td>
        <td rowspan="6">Font set by <a href="">Root.SetFontFamily</a> method</td>
    </tr>
    <tr>
        <td>$FONT3</td>
        <td>3</td>
    </tr>
    <tr>
        <td>$FONT4</td>
        <td>4</td>
    </tr>
    <tr>
        <td>$FONT5</td>
        <td>5</td>
    </tr>
    <tr>
        <td>$FONT6</td>
        <td>6</td>
    </tr>
    <tr>
        <td>$FONT7</td>
        <td>7</td>
    </tr>
</table>

**<small>The Mincho constant has changed from $BOLD to $FONT1 since Version 4.1.0. <br>$BOLD constant compatibility is valid</small>**
<br>**<small>Added constants for $FONT2-7 since Version 4.1.0</small>**
<br>**<small>Not supported in Mobile</small>**
<br>**<small>$FONT2-7 constants are not supported in AI</small>**
