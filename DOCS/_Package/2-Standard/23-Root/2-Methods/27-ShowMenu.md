---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.ShowMenu Property
nav_order: 27
permalink: /package/standard/root/methods/showmenu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specifies whether to show or hide the menu bar of the root window.<br><br>The menu is displayed in the initial state immediately after startup. It returns to the initial state when the <a href="/package/standard/root/methods/login">Login</a> and <a href="/package/standard/root/methods/logout">Logout</a> methods are executed. This method does nothing if Biz / Browser is running inside Internet Explorer.<br><br><b><i>Mobile version , Android version</i></b><br>Specifies the display of the command bar and status bar. The display / non-display state can be changed by specifying a value for mode. It is displayed in the initial state immediately after startup.<br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.2.0.0, AI Ver.1.0.1</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.ShowMenu( <b>flag</b> )<br>Mobile, Android Version<br>//.ShowMenu( <b>mode</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>boolean <b>flag</b></td>
    <td>Specify $ TRUE to display the menu.Specify $ FALSE to hide the menu.<br></td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
    <td><br><br><b><i>Mobile version , Android version</i></b><br>Specify with a combination of the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-34fe{background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">Constant</th>
    <th class="tg-34fe">Value</th>
    <th class="tg-llyw">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Root.Hide</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">non-representation</td>
  </tr>
  <tr>
    <td class="tg-0pky">Root.CommandBar</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Show command bar</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.StatusBar</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Show status bar</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.TaskBar</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">Show taskbar<br>(Windows Mobile only )<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add310.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.SIPBar</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">Show SIP bar<br>(Windows Mobile only )<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add310.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.TitleBar</td>
    <td class="tg-baqh">16</td>
    <td class="tg-0lax">Show title bar<br>(Android version only )<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add101.gif" alt="Image" width="65" height="12"></td>
  </tr>
</tbody>
</table><br><br><small><span style="color:green">It has been changed to the following specifications since Mobile Ver.3.1.0</span></small><br>In the Windows Mobile version, the behavior when Root.Hide is specified has been changed.<br>In previous versions, the taskbar and commandbar were not hidden when Root.Hide was specified, but they are all hidden and Biz / Browser is full screen.<br>Specify Root.TaskBar + Root.SIPBar to display the same as the previous version.<br>Also , the specification of Root.SIPBar takes precedence over the specification of Root.CommandBar , and if Root.SIPBar is not specified, the command bar will not be displayed regardless of the specification of Root.CommandBar.<br>If Root.SIPBar is specified, the command bar will be displayed regardless of Root.CommandBar specified, but if only Root.SIPBar is specified, the menu will not be displayed.<br>The operation of the combination of Root.CommandBar and Root.SIPBar is as follows.<br> <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-2gq6{background-color:#D9D9D9;border-color:inherit;font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-2gq6">Mode</th>
    <th class="tg-kg9c">Action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">None</td>
    <td class="tg-0pky">Hide command bar</td>
  </tr>
  <tr>
    <td class="tg-0pky">Root.CommandBar</td>
    <td class="tg-0pky">Hide command bar</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.SIPBar</td>
    <td class="tg-0lax">Command bar display, menu hiding</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.CommandBar + Root.SIPBar</td>
    <td class="tg-0lax">Command bar display, menu display</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.ShowMenu($FALSE);
 
    Mobile, Android Version
    //.ShowMenu(Root.CommandBar + Root.StatusBar + Root.SIPBar);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/showstatusbar">ShowStatusBar</a> event</td>
  </tr>
</table>



