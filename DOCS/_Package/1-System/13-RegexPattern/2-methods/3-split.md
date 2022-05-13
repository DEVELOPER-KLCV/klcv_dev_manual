---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Split Method
nav_order: 3
permalink: /package/system/regexpattern/methods/split
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets a String array split based on the match between the regular expression pattern and the input string<br>The following is an example of splitting "a--/ cde / f--".
    <table>
      <tr>
        <td>Regular expressions</td>
        <td>limit</td>
        <td>result</td>
      </tr>
      <tr>
        <td>/ /</td>
        <td>2</td>
        <td>"a--", "cde / f--"</td>
      </tr>
      <tr>
        <td>/ /</td>
        <td>Ten</td>
        <td>"a--", "cde", "f--"</td>
      </tr>
      <tr>
        <td>/ /</td>
        <td>-1</td>
        <td>"a--", "cde", "f--"</td>
      </tr>
      <tr>
        <td>――――</td>
        <td>Five</td>
        <td>"a", "", "/ cde / f", "", ""</td>
      </tr>
      <tr>
        <td>――――</td>
        <td>-2</td>
        <td>"a", "", "/ cde / f", "", ""</td>
      </tr>
      <tr>
        <td>――――</td>
        <td>0</td>
        <td>"a", "", "/ cde / f"</td>
      </tr>
    </table>
    </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = rp.Split( <b>input</b> [, <b>limit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">An array of String objects that split the <b>input</b> based on the match<br>The last element of the array contains the string after the last matched position.<br><small>Since Ver.5.0.1, UString type array is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.
 
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>input</b></td>
    <td>Matching input string<br><small>Since Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>
  <tr>
    <td>integer <b>limit</b></td>
    <td>Maximum number of divisions<br>If greater than 0 , the returned array length will be less than or equal to <b>limit</b><br>Negative values ​​do not limit the length of the array.<br>If 0 , the length of the array is not limited, but the following empty string is discarded. If omitted, it will be 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("/");
var arr = p.Split("Biz/Browser");
for (var i = 0; i < arr.length; i++) {
    print(arr[i], "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>

