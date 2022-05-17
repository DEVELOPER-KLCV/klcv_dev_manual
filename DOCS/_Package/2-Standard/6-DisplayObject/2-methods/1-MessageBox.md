---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.MessageBox Method
nav_order: 1
permalink: /package/standard/displayobject/methods/messagebox
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Display a message box.<br><br>An event occurs in response to the button pressed displayed in the message box, and the same value as the event is returned.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.MessageBox( <b>message</b> [, <b>title</b> [, <b>flag</b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">If you select the OK button, OkSelected is returned.<br>If you select the Cancel button , CancelSelected is returned.<br>If you select the Yes button , YesSelected is returned.<br>If you select the No button , NoSelected is returned.<br>If you select the Retry button , RetrySelected is returned.</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>message</b></td>
    <td>The character string to be displayed in the message box</td>
  </tr>
  <tr>
    <td>String <b>title</b></td>
    <td>Message box title</td>
  </tr>
  <tr>
    <td>intger <b>flag</b></td>
    <td>Select the type of button and icon to be displayed in the message box from the following, and specify by adding.<br>For example, if you want to display the OK button and Cancel button and display the ? Icon, specify as follows.<br><br><code><pre>$ OKCANCEL + $ ICONQUESTION</pre></code><br><br>If the button is omitted, it will be the same as $ OK. If the icon is omitted, it will be the same as $ ICONINFOMATION<br><br>Select one button type from the following.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-kg9c">Buttons displayed</th>
    <th class="tg-xt05">Events that occur</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ OK</td>
    <td class="tg-0pky">OK</td>
    <td class="tg-0lax">OkSelected</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ OKCANCEL</td>
    <td class="tg-0pky">OK , Cancel</td>
    <td class="tg-0lax">OkSelected,<br>CancelSelected</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ YESNO</td>
    <td class="tg-0pky">Yes, No</td>
    <td class="tg-0lax">YesSelected,<br>NoSelected</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ RETRYCANCEL</td>
    <td class="tg-0pky">Retry , Cancel</td>
    <td class="tg-0lax">RetrySelected,<br>CancelSelected</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ YESNOCANCEL<br>Added since<br><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add400.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add300.gif" alt="Image" width="86" height="12"><br></td>
    <td class="tg-0lax">Yes, No, Cancel</td>
    <td class="tg-0lax">YesSelected,<br>NoSelected,<br>CancelSelected</td>
  </tr>
</tbody>
</table>
    
    Select one of the displayed icons from the following.<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-8r26">Icon displayed</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ IconInformation</td>
    <td class="tg-c3ow"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjm1.files/image003.png" width="40" height="40"></td>
  </tr>
  <tr>
    <td class="tg-0pky">$ IconQuestion</td>
    <td class="tg-c3ow"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjm1.files/image004.png" width="40" height="40"></td>
  </tr>
  <tr>
    <td class="tg-0pky">$ IconExclamation</td>
    <td class="tg-c3ow"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjm1.files/image005.png" width="40" height="40"></td>
  </tr>
  <tr>
    <td class="tg-0pky">$ IconStop</td>
    <td class="tg-c3ow"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjm1.files/image006.png" width="40" height="40"></td>
  </tr>
</tbody>
</table>

<p style="color:green"><small>You can now specify from 4 types of icons displayed from Mobile Ver.2.0.0.</small></p><br>

Select one of the default buttons below.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ DefButton1</td>
    <td class="tg-0pky">The first button from the left is the default button</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DefButton2</td>
    <td class="tg-0pky">The second from the left is the default button</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DefButton3</td>
    <td class="tg-0pky">The third from the left is the default button</td>
  </tr>
</tbody>
</table>

<p style="color:red"><small>Added since Mobile Ver.4.0.0, Mobile Ver.3.0.0</small></p>
    
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (MessageBox("Please confirm", "Confirm", $OKCANCEL) == OkSelected) {
    :
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/displayobject/events/okselected">OkSelected</a>, <a href="/package/standard/displayobject/events/cancelselected">CancelSelected</a>, <a href="/package/standard/displayobject/events/yesselected">YesSelected</a>, <a href="/package/standard/displayobject/events/noselected">NoSelected</a>, <a href="/package/standard/displayobject/events/retryselected">RetrySelected</a> events</td>
  </tr> 