---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Compile Method
nav_order: 4
permalink: /package/system/regexpattern/methods/compile
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Compile the regular expression to create a RegexPattern object.This method is a static method. You can call it without creating an object.<br></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var rp = RegexPattern.Compile( <b>regex</b> [, <b>flags</b> [, <b>mode</b> ]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">RegexPattern object</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>regex</b></td>
    <td>Regular expressions<br><small>Since Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a></small></td>
  </tr>
  <tr>
    <td>integer <b>flags</b></td>
    <td>Match flag<br>Specify a combination of the following values.
    <table>
      <tr>
        <td>Constant</td>
        <td>Value</td>
        <td>Description</td>
      </tr>
      <tr>
        <td>RegexPattern.CASELESS<br>RegexPattern.CASE_INSENSITIVE</td>
        <td>1</td>
        <td>Performs case-insensitive matching</td>
      </tr>
      <tr>
        <td>RegexPattern.MULTILINE</td>
        <td>2</td>
        <td>The metacharacters "^" and "$" will now match relative to the newline code ( "\n" ).</td>
      </tr>
      <tr>
        <td>RegexPattern.DOTALL</td>
        <td>Four</td>
        <td>The metacharacter "." Will now match all characters, including newlines</td>
      </tr>
      <tr>
        <td>RegexPattern.EXTENDED<br>RegexPattern.COMMENTS</td>
        <td>8</td>
        <td>Whitespace is ignored and lines starting with # are ignored as comments until the end of the line</td>
      </tr>
      <tr>
        <td>RegexPattern.ANCHORED</td>
        <td>16 16</td>
        <td>Limited to match only from the beginning</td>
      </tr>
      <tr>
        <td>RegexPattern.DOLLAR_ENDONLY</td>
        <td>32</td>
        <td>The metacharacter "$" will now match only at the end of the searched string</td>
      </tr>
      <tr>
        <td>RegexPattern.UNGREEDY</td>
        <td>512</td>
        <td>Make repeat specifiers ungreedy by default</td>
      </tr>
    </table>
    If omitted, it is 0 (not specified).
    </td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
    <td>If you want to generate the regular expression engine in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a> , specify RegexPattern.Unicode.<br>If omitted, it is 0 (normal mode). <br><small>Added since Ver.5.0.1</small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 4</td>
    <td>The argument value is invalid</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)", RegexPattern.CASELESS, RegexPattern.Unicode);
var m = p.Matcher("Biz/Browser");
if (m.Matches()) {
    print(m.Group(1), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexpattern/methods/matches">Matches</a> method</td>
  </tr>
</table>
