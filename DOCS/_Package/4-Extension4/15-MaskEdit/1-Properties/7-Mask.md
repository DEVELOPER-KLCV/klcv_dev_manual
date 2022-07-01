---
layout: default

grand_parent: MaskEdit Class
parent: Properties
has_children: false
title: MaskEdit.Mask Property
nav_order: 7
permalink: /package/extension4/maskedit/properties/mask
---
# {{ page.title }}

A mask string that determines the editing behavior of mask edit.

For the mask string, specify a combination of mask characters, control characters, and literal characters for editing. Please refer to the table below for details.

Example

"009999-0999-000"   Phone number <br>
"000-0000"          Postal code <br>
"9999年99月99日"  Date <br>
"Seri￥￥a￥￥l No."    When using escape <br>

***Mask Characters***<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Characters</th>
    <th class="tg-0pky">Required input</th>
    <th class="tg-0pky">Characters that can be entered</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">#</td>
    <td class="tg-c3ow"> </td>
    <td class="tg-0pky">Half - width numbers ( 0-9 )<br>'-' , '+' sign,<br>Half-width space</td>
  </tr>
  <tr>
    <td class="tg-0pky">0</td>
    <td class="tg-c3ow">○</td>
    <td class="tg-0pky" rowspan="2">Half - width numbers ( 0-9 )</td>
  </tr>
  <tr>
    <td class="tg-0pky">9</td>
    <td class="tg-c3ow"> </td>
  </tr>
  <tr>
    <td class="tg-0pky">A ( capital )</td>
    <td class="tg-c3ow">○</td>
    <td class="tg-0pky" rowspan="2">Half-width alphabetic characters ( A to Z , a to z )<br>Half - width numbers ( 0-9 )</td>
  </tr>
  <tr>
    <td class="tg-0pky">a ( small text )</td>
    <td class="tg-c3ow"> </td>
  </tr>
  <tr>
    <td class="tg-0pky">L ( large text ) , ?</td>
    <td class="tg-c3ow">○</td>
    <td class="tg-0pky" rowspan="2">Half-width alphabetic characters ( A to Z , a to z )</td>
  </tr>
  <tr>
    <td class="tg-0pky">l ( small text )</td>
    <td class="tg-c3ow"> </td>
  </tr>
  <tr>
    <td class="tg-0pky">C ( large text ) , &amp;</td>
    <td class="tg-c3ow">○</td>
    <td class="tg-0pky" rowspan="2">Any half-width character<br>However, if C is repeated more than once, you can also enter double-byte characters .<br><b><i>Mobile version</i></b><br>You can enter both full-width and half-width characters for one C.</td>
  </tr>
  <tr>
    <td class="tg-0pky">c ( small text )</td>
    <td class="tg-c3ow"> </td>
  </tr>
</tbody>
</table>

***Control characters***<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow">Characters</th>
    <th class="tg-0pky">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">&lt; </td>
    <td class="tg-0pky">Convert the letters after this symbol to lowercase and enter. (Full-width alphabets are not converted)</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&gt; </td>
    <td class="tg-0pky">Enter the letters after this symbol by converting them to uppercase. (Full-width alphabets are not converted)</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&lt;&gt; </td>
    <td class="tg-0pky">After this symbol, disable case conversion and follow the keystrokes.</td>
  </tr>
  <tr>
    <td class="tg-c3ow">\</td>
    <td class="tg-0pky">The escape character. Treats the next one character as an editing literal character.<br>Example）￥A, ￥0, ￥&lt;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">;</td>
    <td class="tg-0pky">This is the delimiter when a blank character is specified.</td>
  </tr>
</tbody>
</table>

***Editing literal characters***<br>
Characters other than the above are retail characters for editing.
The cursor is automatically skipped. It cannot be deleted or changed by screen operation.

***Half-width conversion of full-width characters***<br>
If you enter a full-width character in the half-width character input field, it will be automatically converted to a half-width character.
Full-width characters to be converted are alphanumeric characters, + sign,-sign, and space.

<small><span style="color:green">The following full-width symbol characters are also converted since Ver.5.0.0.<br>!! "# $% &'() * +,-./:; <=>? @ [\] ^ _'{|}</span></small>

***Specify blank characters***<br>
By specifying a semi-colon ";" and one half-width character at the end of the mask character string, you can change the blank character displayed at the unentered position.
This specification can be omitted, otherwise it will be an underscore "_".

Example

"009999-0999-000; *"
 
The character used for the blank character can be entered as an input value, but it is not possible to determine whether the character specified for the blank character is set by key input or not.