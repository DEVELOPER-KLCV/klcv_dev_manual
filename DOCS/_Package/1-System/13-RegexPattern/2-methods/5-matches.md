---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Matches Method
nav_order: 5
permalink: /package/system/regexpattern/methods/matches
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Matches the specified regular expression and input string.<br>This method is a static method. Can be called without creating an object.<br><br>This method allows you to perform a match without having to go through the steps of creating an object.<br>The next two statements give similar results.<br><br><code><pre>RegexPattern.Matches ("[0-9] + / [0-9] + / [0-9] +", "2011/11/28"); <br>RegexPattern.Compile ("[0-9] + / [0-9] + / [0-9] +"). Matcher ("2011/11/28"). Matches ();</pre></code><br><br>If you use the same regular expression repeatedly, it is more efficient to create the object with the <a href="/package/system/regexpattern/methods/compile">Compile</a> method than to call this method every time.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = RegexPattern.Matches( <b>regex</b>, <b>input</b> [, <b>flags</b> [, <b>mode</b> ]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$ TRUE if it matches, $ FALSE if it doesn't</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>String <b>regex</b></td>
    <td>Regular expressions<br><small>Since Ver.5.0.1, UString type array is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>
  
  <tr>
    <td>String <b>input</b></td>
    <td>Matching input string<br><small>Since Ver.5.0.1, UString type array is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>
  <tr>
    <td>integer <b>flags</b></td>
    <td>Match flag<br>See <a href="/package/system/regexpattern/methods/compile">Compile</a> method for details.<br>If omitted, it is 0 (not specified).</td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
    <td>If you want to generate the regular expression engine in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>, specify RegexPattern.Unicode</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 4</td>
    <td>The argument value is invalid</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (RegexPattern.Matches("[0-9]+/[0-9]+/[0-9]+", "2011/11/28")) {
    //.MessageBox("Matched");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexpattern/methods/compile">Compile</a>, <a href="/package/system/regexpattern/methods/matcher">Matcher</a> method</td>
  </tr>

