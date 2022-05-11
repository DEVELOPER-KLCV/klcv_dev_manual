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
    <td>Regular expressions<br><small>Since Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern">Unicode mode</a></td>
  </tr>
  <tr>
    <td>integer <b>flags</b></td>
    <td>Match flag<br>Specify a combination of the following values.
      <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-dwjs{background-color:#d9d9d9;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-bkvp{background-color:#d9d9d9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-dwjs">Constant</th>
    <th class="tg-bkvp">Value</th>
    <th class="tg-bkvp">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">RegexPattern.CASELESS<br>RegexPattern.CASE_INSENSITIVE</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">Performs case-insensitive matching</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.MULTILINE</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">The metacharacters "^" and "$" will now match relative to the newline code ( "\ n" ).</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.DOTALL</td>
    <td class="tg-0lax">Four</td>
    <td class="tg-0lax">The metacharacter "." Will now match all characters, including newlines</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.EXTENDED<br>RegexPattern.COMMENTS</td>
    <td class="tg-0lax">8</td>
    <td class="tg-0lax">Whitespace is ignored and lines starting with # are ignored as comments until the end of the line</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.ANCHORED</td>
    <td class="tg-0lax">16 16</td>
    <td class="tg-0lax">Limited to match only from the beginning</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.DOLLAR_ENDONLY</td>
    <td class="tg-0lax">32</td>
    <td class="tg-0lax">The metacharacter "$" will now match only at the end of the searched string</td>
  </tr>
  <tr>
    <td class="tg-0lax">RegexPattern.UNGREEDY</td>
    <td class="tg-0lax">512</td>
    <td class="tg-0lax">Make repeat specifiers ungreedy by default</td>
  </tr>
</tbody>
</table>
    
    If omitted, it is 0 (not specified).
    </td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
    <td>If you want to generate the regular expression engine in Unicode mode , specify RegexPattern.Unicode.<br>If omitted, it is 0 (normal mode). <small>Added since Ver.5.0.1</small></td>
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
