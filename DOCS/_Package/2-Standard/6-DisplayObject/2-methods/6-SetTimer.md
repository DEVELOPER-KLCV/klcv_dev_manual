---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.SetTimer Method
nav_order: 6
permalink: /package/standard/displayobject/methods/settimer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.SetTimer( <b>sec</b> [, <b>oneshot</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>sec</b></td>
    <td></td>
  </tr>
  <tr>
    <td>boolean <b>oneshot</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
SetTimer(2.5);
var count = 0;
Function OnTimer(e) {
    count++;
    if (count >= 5) {
        RemoveTimer();
    }
    print(sysdate(), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/displayobject/methods/removetimer">RemoveTimer</a> method<br><a href="/package/standard/displayobject/events/timer">Timer</a> event</td>
  </tr>
</table>

