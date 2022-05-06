---
layout: default

parent: 1. String Manipulation

title: strf
nav_order: 12
permalink: /method/str/strf
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Replaces %n that appears in the <b>format string</b> with the string specified by the subsequent argument <b>str_n</b>.<br>%n specifies the next argument of the format string as %1 and the next as %2.<br><br>If there are fewer arguments than %n, it is assumed that an empty string was specified and %n is deleted.<br><br>If you want to include the character "%" in the format string, specify it in duplicate like "%%".<br>However, if % is not followed by a number,% is output as is.<br><br>*<small>Added since Version 4.1.0</small>*<br>*<small>Cannot be used with Mobile version</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = strf( <b>formatting string</b> [, <b>str_1</b> [, <b>str_2</b>, ... ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced string</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>Formatting string</b></td>
    <td>Formatted string</td>
  </tr>
  <tr>
    <td>String <b>str_n</b></td>
    <td>String to replace</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var filename = "sample.txt";
MessageBox(strf("「%1」を削除します。よろしいですか？", filename), "確認", $OKCANCEL);
 
var y = 2011;
var m = 9;
var p = 120;
print(strf("%1年%2月の売上げ前年比は%3%%です\n", y, m, p));
 
var d = sysdate();
print(strf("今日は%1年%2月%3日です\n", year(d), month(d), day(d)));
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

