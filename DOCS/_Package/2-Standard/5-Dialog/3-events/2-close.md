---
layout: default

grand_parent: Dialog Class
parent: Events
has_children: false
title: Dialog.Close Event
nav_order: 2
permalink: /package/standard/dialog/events/close
---
# {{ page.title }}

Occurs when pressing the close button in the upper right corner of the dialog.

If this event is caught by the event handler, the action of closing the dialog will be cancelled. To close the dialog, delete the Dialog object in the event handler.

Example
```
Function OnClose (e) {
    if (...) {
        Dialog1.Delete ();
    }
}
```
<p style="color:red;"><small>The following specifications have been added to AI--></small></p>

In the Android version, the following objects are added as child objects of the Event object.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-6t3r{font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-xt05">Name</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">CauseClose</td>
    <td class="tg-0lax">A value that describes how the Dialog is about to be closed.<br> </td>
  </tr>
</tbody>
</table>

CauseClose contains the following constant values ​​that indicate how it is about to be closed.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant name</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Meaning</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Dialog.CLOSE_ON_BACK_KEY</td>
    <td class="tg-ihln">1</td>
    <td class="tg-0lax">When you try to close by pressing the Back key of Android</td>
  </tr>
  <tr>
    <td class="tg-0lax">Dialog.CLOSE_ON_TOUCH_OUTSIDE</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">When you try to close by tapping outside the dialog<br>( Only occurs on Android 3.x and above )</td>
  </tr>
</tbody>
</table>

Example

```
Function OnClose (e) {
    if (e.CauseClose == Dialog.CLOSE_ON_BACK_KEY) {
        / * Closes the dialog only when the "Back" button on the terminal is pressed * /
        Dialog1.Delete ();
    }
}
```
<p style="color:red;"><small><--Up to here</small></p>