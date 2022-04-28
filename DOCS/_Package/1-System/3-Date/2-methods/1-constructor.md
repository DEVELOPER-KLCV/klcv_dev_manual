---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date constructor
nav_order: 1
permalink: /package/system/date/methods/constructor
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the Date object.<br><br>If no arguments are taken, it will be initialized with the current date and time.<br><br>When one argument is specified, if the argument is a character string representing date / time, the same interpretation as the parse method is performed, otherwise the date and time are initialized as milliseconds representing the elapsed time from UTC reference time increase.<br>See <a href="/package/system/date/methods/parse">parse</a> method for string format<br><br>If two or more arguments are specified, up to seven will be initialized as year, month, day, hour, minute, second, and millisecond (actually invalid).All omitted arguments will be 0.<br><br>Creating a Date object without a constructor call will create a Date object with an invalid date and time without being initialized.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = new Date( )<br>var d = new Date(<b>value</b>)<br>var d = new Date(<b>year, month, date [, hours [, minute [, sec [, ms ] ] ] ]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Date object</td>
  </tr>  
  <tr>
    <td rowspan="8">Arguments</td>
    <td>Object <b>value</b></td>
    <td>An object that represents a date string or elapsed time</td>
  </tr>
  <tr>
    <td>integer <b>year</b></td>
    <td>Specify the year numerically</td>
  </tr>
  <tr>
    <td>integer <b>month</b></td>
    <td>Specify the month number with January as 0</td>
  </tr>
  <tr>
    <td>integer <b>date</b></td>
    <td>Specify the day numerically</td>
  </tr>
  <tr>
    <td>integer <b>hours</b></td>
    <td>Specify the hour numerically</td>
  </tr>
  <tr>
    <td>integer <b>minute</b></td>
    <td>Specify the minute numerically</td>
  </tr>
  <tr>
    <td>integer <b>sec</b></td>
    <td>Specify the seconds numerically</td>
  </tr>
    <tr>
    <td>integer <b>ms</b></td>
    <td>Ignored</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d1 = new Date ();
var d2 = new Date (1964, 8, 10);
var d3 = new Date ("2002/01/02 12:34:56");
var d4 = new Date (1022889600000);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/date/methods/parse">parse</a> method</td>
  </tr>
</table>


