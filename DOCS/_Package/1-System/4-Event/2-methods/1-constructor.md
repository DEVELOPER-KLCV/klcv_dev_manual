---
layout: default

grand_parent: Event Class
parent: Methods
has_children: false
title: Event Constructor
nav_order: 1
permalink: /package/system/event/methods/constructor
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the Event object.<br>If you specify a <b>reason</b>, it initializes the Reason property.<br>If you specify <b>eventName</b>, it initializes the EventName property.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ev = new Event( <b>[ reason [, eventName ] ]</b> )<br>OR<br>var ev = new Event( <b>eventName</b> ) <br> <small> Added since Ver.4.0.0 and Mobile Ver.3.2.0</small></td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Event object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>reason</b></td>
    <td>Specify the event type numerically. For user-specific events, specify a value greater than UserEvent.</td>
  </tr>
  <tr>
    <td>String <b>eventName</b></td>
    <td>Specify the name of the event.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnSampleEvent (e) {
    print ("Event.Reason =", e.Reason, "￥ n");
    print ("Event.EventName =", e.EventName, "￥ n");
    print ("Event.From.Name =", e.From.Name, "￥ n");
}
PostEvent (new Event (UserEvent + 1, "SampleEvent"));</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



