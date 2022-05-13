---
layout: default

grand_parent: Dialog Class
parent: Methods
has_children: false
title: Dialog.SetWindowState Method
nav_order: 5
permalink: /package/standard/dialog/methods/setwindowstate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Maximize and minimize the dialog and change the context.<br><small>Added since Ver.4.1.3<br>Not supported in Mobile, AI</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Dialog1.SetWindowState( <b>state</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>state</b></td>
    <td>Specify the settings related to the size of the dialog and the settings related to the context.<br>If both are specified at the same time, the values will be added. ($ MAXMIZE + $ FRONT, etc.)<br><br>Specify the size status with one of the values ​​below.
        <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
 <table class="tg">
  <thead>
     <tr>
     <th class="tg-kg9c">Constant</th>
     <th class="tg-2m49">Value</th>
     <th class="tg-xt05">Description</th>
     </tr>
  </thead>
  <tbody>
     <tr>
     <td class="tg-0pky">$ MINIMIZE</td>
     <td class="tg-baqh">1</td>
     <td class="tg-0lax">Minimize</td>
     </tr>
     <tr>
     <td class="tg-0pky">$ MAXIMIZE</td>
     <td class="tg-baqh">2</td>
     <td class="tg-0lax">Maximize</td>
     </tr>
     <tr>
     <td class="tg-0lax">$ RESTORE</td>
     <td class="tg-baqh">3</td>
     <td class="tg-0lax">If it is currently maximized or minimized,  restore it.</td>
     </tr>
     <tr>
     <td class="tg-0lax">$ FULLSCREEN</td>
     <td class="tg-baqh">32</td>
     <td class="tg-0lax">Moves to full screen display mode without title bar<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add502.gif" alt="Image" width="50" height="12"></td>
     </tr>
   </tbody>
  </table>


   Specify the context with one of the values ​​below.
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ FRONT</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">Move the window to the table</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ BACK</td>
    <td class="tg-baqh">16 16</td>
    <td class="tg-0lax">Move the window to the back</td>
  </tr>
</tbody>
</table>
    </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
Dialog1.SetWindowState($MAXIMIZE + $FRONT);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/dialog/events/windowstatechanged">WindowStateChanged</a> event</td>
  </tr>
</table>