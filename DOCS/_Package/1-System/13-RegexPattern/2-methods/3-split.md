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
       <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-rkel{background-color:#c0c0c0;border-color:#343434;text-align:left;vertical-align:top}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-vckx{background-color:#c0c0c0;border-color:#343434;font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-ur59{border-color:#343434;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-f7v4">Regular expressions</th>
    <th class="tg-vckx">limit</th>
    <th class="tg-rkel">result</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-73oq">/ /</td>
    <td class="tg-ur59">2</td>
    <td class="tg-ur59">"a--", "cde / f--"</td>
  </tr>
  <tr>
    <td class="tg-73oq">/ /</td>
    <td class="tg-ur59">Ten</td>
    <td class="tg-ur59">"a--", "cde", "f--"</td>
  </tr>
  <tr>
    <td class="tg-73oq">/ /</td>
    <td class="tg-ur59">-1</td>
    <td class="tg-ur59">"a--", "cde", "f--"</td>
  </tr>
  <tr>
    <td class="tg-73oq">――――</td>
    <td class="tg-ur59">Five</td>
    <td class="tg-ur59">"a", "", "/ cde / f", "", ""</td>
  </tr>
  <tr>
    <td class="tg-73oq">――――</td>
    <td class="tg-ur59">-2</td>
    <td class="tg-ur59">"a", "", "/ cde / f", "", ""</td>
  </tr>
  <tr>
    <td class="tg-73oq">――――</td>
    <td class="tg-ur59">0</td>
    <td class="tg-ur59">"a", "", "/ cde / f"</td>
  </tr>
</tbody>
</table>
    
    
    </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = rp.Split( <b>input</b> [, <b>limit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">An array of String objects that split the <b>input</b> based on the match<br>The last element of the array contains the string after the last matched position.<br><small>Since Ver.5.0.1, UString type array is returned in <a href="/package/system/regexpattern">Unicode mode</a>.
 
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>input</b></td>
    <td>Matching input string<br><small>Since Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern">Unicode mode</a>
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

