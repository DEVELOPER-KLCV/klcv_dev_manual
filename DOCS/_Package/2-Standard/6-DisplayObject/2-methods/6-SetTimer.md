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
    <td colspan="2">Raises a <a href="/package/standard/displayobject/events/timer">Timer</a> event at sec intervals. One timer can be set for one object. The timer resolution is 0.1 seconds.<br><br>If you set a timer, the event will occur repeatedly at specified intervals. Call the <a href="/package/standard/displayobject/methods/removetimer">RemoveTimer</a> method to remove the set timer.<br><br>If the sec interval is shorter than the time required to process the OnTimer event handler, Timer events may accumulate in the event queue and become inoperable. Pay close attention to the specified interval of sec.<br><br>Also, if you write the <a href="/package/standard/displayobject/methods/removetimer">RemoveTimer</a> method in the Timer event with the expectation that it will be executed only once, if you specify a very short sec interval, the next Timer event will occur before the <a href="/package/standard/displayobject/methods/removetimer">RemoveTimer</a> method in the Timer event is executed. Be sure to specify oneshot as $ TRUE for a one-time execution.<br><small><p style="color:green">Calling the SetTimer method is invalid for Doc objects and their child objects from Ver.4.0.5. <br>No error will occur, but the Timer event will not occur.<br>From Ver.5.0.0, the resolution of the timer has been expanded from 0.1 seconds to 0.01 seconds.</p></small></td>
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
    <td>Specifies the timer event issuance interval in seconds.</td>
  </tr>
  <tr>
    <td>boolean <b>oneshot</b></td>
    <td>Specifying $ TRUE raises the Timer event only once. In this case, you don't need to call the RemoveTimer method.<br>The default is $ FALSE.<br>
    <small><p style="color:red">Added since Ver.5.0.0</p></small> <small><p style="color:blue">Not supported in Mobile</p></small> </td>
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


