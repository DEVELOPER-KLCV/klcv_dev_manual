---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.Dial Property
nav_order: 30
permalink: /package/standard/root/methods/dial
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Make dial-up connection and disconnection.<br><br>For Windows CE, if the <a href="/package/standard/root/properties/dialentry">DialEntry</a> property is specified, the connection name is used, and if not specified, the setting value of "Auto dial name" in "Internet options" is used. <br> It is also affected by the Root.Silent specification specified in the <a href="/package/standard/root/properties/autodial">AutoDial</a> property.<br><small><span style="color:red">Can only be used with Mobile<br>Only supported since Mobile Ver3.2.1</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = //.Dial( <b>action</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns $ TRUE on success, $ FALSE if the connection (disconnect) fails or is already connected (disconnected).<br> Always returns $ TRUE if action is Root.DownAlt.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>action</b></td>
    <td>Specify one of the following values.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7jy7">Constant</th>
    <th class="tg-7jy7">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Root.UP</td>
    <td class="tg-0pky">Make a dial-up connection</td>
  </tr>
  <tr>
    <td class="tg-0pky">Root.Down</td>
    <td class="tg-0pky">Disconnect</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.DownAlt</td>
    <td class="tg-0lax">It is effective only for Windows Mobile. Click the "End call" button to disconnect.<br>It is considered the same as Down on Windows CE.<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add322.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Root.CommandBar + Root.SIPBar</td>
    <td class="tg-0lax">Command bar display, menu display</td>
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
    <td colspan="2">
    <code><pre>
    //.Dial(Root.UP);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/properties/autodial">AutoDial</a>, <a href="/package/standard/root/properties/dialentry">DialEntry</a> properties</td>
  </tr>
</table>



