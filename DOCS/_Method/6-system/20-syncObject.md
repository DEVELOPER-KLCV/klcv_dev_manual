---
layout: default

parent: 6. System Functions

title: syncObject
nav_order: 20
permalink: /method/system/syncObject
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">In Biz / Browser , the script execution engine and GUI operations are thread-separated and executed asynchronously to improve performance.Therefore , the value is reflected to the GUI asynchronously after the script is executed. As a negative effect, it is not possible to write coding that works by confirming that the GUI state is changed during script execution. <br><br>Use this function to synchronize the state to the GUI immediately. By performing state synchronization, it is possible to perform coding that is aware of changes in the GUI in the script. <br><p style="color:red;">Precautions for use</p> This function forces a normal Biz / Browser behavior sequence change. If it is executed continuously in a loop, it may cause problems such as poor performance and incorrect GUI update. <br> It is reccommended to use it at one point as much as possible.<br><br><small>Added since Ver.5.0.0<br>Not available in Mobile</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">syncObject ()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnTouch (e) {
    / * Display dialog during processing * /
    Get ("Dialog1.crs");
    
    / * Synchronize GUI to display dialog * /
    syncObject ();
        
    / * Time-consuming processing * /
    var COUNT = 1000;
    for (var i = 0; i <COUNT; i ++) {
        / * Processing execution * /
    }
    / * Delete dialog * /
    Dialog1.Delete ();
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





