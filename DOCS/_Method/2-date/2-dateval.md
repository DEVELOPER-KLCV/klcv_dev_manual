---
layout: default

parent: Date Functions

title: dateval
nav_order: 2
permalink: /method/date/dateval
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specifies the format of the <b>date string</b>. Returns 0 if the <b>date string</b> cannot be interpreted as a date.<br>If you do not include the time in the <b>date string</b>, the time will be 0:00:00. If seconds are not included, it will be 0 seconds.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = dateval (<b>date string</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a Date object.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>Date string</b></td>
    <td>Specify one of the following formats:<br>"YY / MM / DD"<br>"YY / MM / DD HH24: MI"<br>"YY / MM / DD HH24: MI: SS"<br>"YYYY / MM / DD"<br>"YYYY / MM / DD HH24: MI"<br>"YYYY / MM / DD HH24; MI: SS"</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = dateval("2002/2/28");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





