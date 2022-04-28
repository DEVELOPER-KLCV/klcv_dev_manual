---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.SetKeywordStyle Method
nav_order: 11
permalink: /package/extension4/styleedit/methods/SetKeywordStyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.SetKeywordStyle( <b>styleNo</b>, <b>keywordsOrRegExp</b>, <b>mode</b>, <b>fgColor</b> [, <b>bgColor</b> [, <b>fontFace</b> [, <b>fontKind</b> [, <b>fontSize</b> ] ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="8">Arguments</td>
    <td>integer <b>styleNo</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>keywordsOrRegExp</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>integer </b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>fgColor </b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>bgColor </b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>fontFace </b></td>
    <td></td>
  </tr>
  
  <tr>
    <td>integer <b>fontKind </b></td>
    <td></td>
  </tr>
  
  <tr>
    <td>integer <b>fontSize </b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td></td>
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
 
The regular expression specifications that can be used in the StyleEdit class are as follows. (Specifications are different from the regular expression of [RegexPattern]() class)

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