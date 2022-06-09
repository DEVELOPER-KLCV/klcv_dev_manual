---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetMemoryLimitThreshold Property
nav_order: 35
permalink: /package/standard/root/methods/setmemorylimitthreshold
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"><br><br> The memory that can be used by Biz / Browser AI is very limited to about 16MB to 48MB like a general Android application, and the maximum memory size differs for each terminal, so it is necessary to pay attention to the amount of memory used.<br><br>Therefore, if the memory usage exceeds the threshold while the threshold is set using this method, the <a href="/package/standard/root/events/memorylimitexceeded">MemoryLimitExceeded</a> event is issued only once and the threshold is reset.<br>If you want to continue to monitor memory usage, call this method again.<br><br> Please take note, even if you set a threshold, if the maximum memory usage is reached by the time the <a href="/package/standard/root/events/memorylimitexceeded">MemoryLimitExceeded</a> event occurs, an OutOfMemory error will occur, so the event will not occur reliably before stopping due to insufficient memory.<br> <br><small><span style="color:red">Added since AI Ver.1.0.1</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetMemoryLimitThreshold( <b>threshold</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Number <b>threshold</b></td>
    <td>Set a threshold for issuing a memory usage warning event.<br>The unit is MB.<br>If 0 or a negative value, reset the threshold setting.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetMemoryLimitThreshold( 24.0 );
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/properties/reloggedin">ReLoggedIn</a> property, <a href="/package/standard/root/events/memorylimitexceeded">MemoryLimitExceeded</a> event</td>
  </tr>
</table>



