---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.SetKeywordStyle Method
nav_order: 11
permalink: /package/extension4/styleedit/methods/setkeywordstyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Register the style and the keyword to be applied in the style number.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.SetKeywordStyle( <b><i>styleNo</i></b>, <b><i>keywordsOrRegExp</i></b>, <b><i>mode</i></b>, <b><i>fgColor</i></b> [, <b><i>bgColor</i></b> [, <b><i>fontFace</i></b> [, <b><i>fontKind</i></b> [, <b><i>fontSize</i></b> ] ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="8">Arguments</td>
    <td>integer <b><i>styleNo</i></b></td>
    <td>The style number to register.<br>The range that can be specified is from 0 to 8.</td>
  </tr>
  <tr>
    <td>String <b><i>keywordsOrRegExp</i></b></td>
    <td>Specify a keyword list or regular expression.<br> The keyword list is a character string in which keywords are separated by one of the characters "\ n", "\ r", "\ t", and a space. <br> Up to 256 keywords can be registered.<br>  Since the condition is applied to the regular expression line by line, you cannot specify a style that spans multiple lines.</td>
  </tr>
  <tr>
    <td>integer <b><i>mode</i></b></td>
    <td>Specifies the behavior of the style.<br>
   <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">StyleEdit.REGEXP</td>
    <td class="tg-j5n6">Interpret the keyword as a regular expression</td>
  </tr>
  <tr>
    <td class="tg-j5n6">StyleEdit.NOCASE</td>
    <td class="tg-j5n6">Case insensitive</td>
  </tr>
  <tr>
    <td class="tg-j5n6">StyleEdit.HOTSPOT</td>
    <td class="tg-j5n6">Specify the hotspots ( mouse clickable style )</td>
  </tr>
  <tr>
    <td class="tg-j5n6">StyleEdit.BRACESTART</td>
    <td class="tg-j5n6">Specify the start keyword for the collapsed paragraph</td>
  </tr>
  <tr>
    <td class="tg-j5n6">StyleEdit.BRACEEND</td>
    <td class="tg-j5n6">Specify the end keyword for the collapsed paragraph</td>
  </tr>
</tbody>
</table><br><small><span style="color:red">StyleEdit.BRACESTART and StyleEdit.BRACEEND have been added from Ver.4.1.3</span></small></td>
  </tr>
  <tr>
    <td>integer <b><i>fgColor</i></b></td>
    <td>Specify the font color with a <a href="/base/color">color constant</a>
.</td>
  </tr>
  <tr>
    <td>integer <b><i>bgColor</i></b></td>
    <td>Specify the background color with a <a href="/base/color">color constant</a>
.</td>
  </tr>
  <tr>
    <td>integer <b><i>fontFace</i></b></td>
    <td>Specifies the decoration attributes of the font.The value follows the FontFace property.</td>
  </tr>
  
  <tr>
    <td>integer <b><i>fontKind</i></b></td>
    <td>Specifies the font type. The value follows the FontKind property.</td>
  </tr>
  
  <tr>
    <td>integer <b><i>fontSize</i></b></td>
    <td>Specifies the font size. The value follows the FontSize property.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid arguments</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    /* keyword list */
    StyleEdit1.SetKeywordStyle(0, "AXISSOFT\nアクシス\nソフト\nbiz-collections", StyleEdit.NOCASE, $RED, $STD, $BOLD, $STD, 14);
    
    /* Display URL in blue, specify hotspot */
    StyleEdit1.SetKeywordStyle(1, "http[s]*://[0-9a-z_/\\.\\-?=&~#:]+", StyleEdit.REGEXP + StyleEdit.NOCASE + StyleEdit.HOTSPOT, $BLUE);
    
    /* Specify BEGIN to END as a folding paragraph */
    StyleEdit1.SetKeywordStyle(5, "BEGIN", StyleEdit.NOCASE + StyleEdit.BRACESTART, $RED);
    StyleEdit1.SetKeywordStyle(6, "END", StyleEdit.BRACEEND, $RED);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/styleedit/methods/setstyle">SetStyle</a>, <a href="/package/extension4/styleedit/methods/resetstyle">ResetStyle</a>  method</td>
  </tr>
</table>

<b>Regular expressions that can be used with StyleEdit</b>
 
The regular expression specifications that can be used in the StyleEdit class are as follows. (Specifications are different from the regular expression of [RegexPattern](/package/system/regexpattern) class)

| .. | Any character |
| [] | One character in parentheses<br>[abc] matches a, b, c.<br>[A-Z] matches all uppercase alphabets. |
| [^] | One character not included in parentheses |
| ^ ^ | Match at the beginning of the line |
| $  | Match at the end of the line |
| &#42; | Repeat 0 or more times of the previous pattern |
| +  | Repeat one or more of the previous pattern |
| \ (\) | The part enclosed by this can be called later with \ n.<br>Numbers starting from 1 are assigned, and the number is specified for n. |
| \ n | Call the part enclosed in \ (\). (N is a number from 1 to 9) |
| \ \ | Escape the metacharacters \ [] * + ^ $ |

Since "\" is also an escape character of CRS script, when writing a regular expression in a script, overlap it like "\\". For example, if you want to match the character \, it will be "\\\\".