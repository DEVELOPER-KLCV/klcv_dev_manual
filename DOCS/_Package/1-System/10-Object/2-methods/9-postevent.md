---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.PostEvent Method
nav_order: 9
permalink: /package/system/object/methods/postevent
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Send an event to the object.<br><br>This method allows the CRS program to raise an event at any time.<br>Events are passed to the corresponding event handler via the event queue.See <a href="/bizBrowserV/3/3-7/">Events and Event Handlers</a> for more information.<br><br>When sending a user-defined event, use the event number of the <a href="package/system/event/properties/reason">Reason</a> property after the code number indicated by UserEvent ( such as UserEvent + 1 ) so that it does not overlap with the system-defined event number.<br><br>When sending a system-defined event, you can specify the event name as is for <b>ev</b>.<br><br>The event can be forwarded to the parent object by calling the PostEvent method in the event handler with no arguments.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.PostEvent( [ <b>ev</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td>None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Event <b>ev</b></td>
    <td><a href="/package/system/event">Event</a> object for user-defined events to send<br>Or system-defined event name<br>If omitted, the event is forwarded to the parent object as it is.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
/* User-defined event */
PostEvent(new Event(UserEvent + 1, "AppEvent1"));
 
/* System-defined event */
PostEvent(Touch);
 
Function OnAppEvent1(e) {
    print("AppEvent1\n");
}
Function OnTouch(e) {
    print("Touch\n");
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/event">Event</a> class</td>
  </tr>
</table>



