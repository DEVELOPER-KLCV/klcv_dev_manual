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
    <td></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.PostEvent( [ <b>ev</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Event <b>ev</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td><code><pre>
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
    <td><a href="/package/system/event">Event</a> class</td>
  </tr>
</table>



