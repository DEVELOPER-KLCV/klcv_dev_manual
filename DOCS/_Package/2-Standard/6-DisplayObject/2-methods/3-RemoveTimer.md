---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.RemoveTimer Method
nav_order: 3
permalink: /package/standard/displayobject/methods/removetimer
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.RemoveTimer( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
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
    <td colspan="2"><a href="/package/standard/displayobject/methods/settimer">SetTimer</a> method<br><a href="/package/standard/displayobject/events/timer">Timer</a> event</td>
  </tr>
</table>

