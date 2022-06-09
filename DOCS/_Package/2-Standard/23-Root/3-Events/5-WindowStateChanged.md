---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.WindowStateChanged Event
nav_order: 5
permalink: /package/standard/root/events/windowstatechanged
---
# {{ page.title }}
<br>

Occurs when state changes occur, such as maximizing or minimizing the root window.

<b><i> PC version, Mobile version</i></b><br>
The following child objects are attached to the Event object.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, Arial;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, Arial;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-rvyq{border-color:inherit;font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-8r26">Name</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-rvyq">state </td>
    <td class="tg-0pky">The following values are set.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-8r26">Value</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ MINIMIZE</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-0pky">Minimized</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ MAXIMIZE</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Maximized</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ RESTORE</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">When the size is other than maximize / minimize</td>
  </tr>
</tbody>
</table></td>
  </tr>
</tbody>
</table>

For the Mobile version, the state value is an OS-dependent constant.

<br><small><span style="color:red">Added since Ver.4.1.3, Mobile Ver.2.0.0</span></small>

<br><small><span style="color:green">Expansion since Mobile Ver.3.2.1-></span></small><br>

An event is fired when the foreground application changes.<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ FRONT</td>
    <td class="tg-lcf4">8</td>
    <td class="tg-0pky">Changed from another application to Biz / Browser Mobile</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ BACK</td>
    <td class="tg-tcrt">16 </td>
    <td class="tg-0lax">Changed from Biz / Browser Mobile to another application</td>
  </tr>
</tbody>
</table>
<br>As an exception, it also occurs when the version information dialog of Biz / Browser Mobile is displayed. <br>

<small><span style="color:green"><-Up to here</span></small><br>

<b><i>Android version</i></b><br>
The following child objects are attached to the Event object.<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-imtw{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-23hc">Name</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-imtw">state </td>
    <td class="tg-0pky">The following values are set.<br>For more information on activities (android.app.Activity class ) and their state transitions , please refer to the Android Developers reference manual.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ RESTORE</td>
    <td class="tg-lcf4">3</td>
    <td class="tg-0pky">When the size of the Root window changes<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add101.gif" alt="Image" width="65" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ACTIVITY_ON_START</td>
    <td class="tg-baqh">33 </td>
    <td class="tg-0lax">When the onStart method of the activity running Biz / Browser AI is called</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ACTIVITY_ON_RESUME</td>
    <td class="tg-baqh">34</td>
    <td class="tg-0lax">When the onResume method of the activity running Biz / Browser AI is called</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ACTIVITY_ON_PAUSE</td>
    <td class="tg-baqh">35</td>
    <td class="tg-0lax">When the onPause method of an activity running Biz / Browser AI is called</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ACTIVITY_ON_STOP</td>
    <td class="tg-baqh">36</td>
    <td class="tg-0lax">When the onStop method of the activity running Biz / Browser AI is called</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ACTIVITY_ON_RESTART</td>
    <td class="tg-baqh">37 </td>
    <td class="tg-0lax">When the onRestart method of the activity running Biz / Browser AI is called</td>
  </tr>
</tbody>
</table>