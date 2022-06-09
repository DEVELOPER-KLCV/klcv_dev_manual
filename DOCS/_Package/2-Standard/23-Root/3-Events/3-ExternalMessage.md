---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.ExternalMessage Event
nav_order: 3
permalink: /package/standard/root/events/externalmessage
---
# {{ page.title }}
<br>

Obtained by <a href="/package/extobjectpackage/extobjjava/methods/getmessagehandler">ExternalObject.GetMessageHandler</a> method<br>

Occurs when sending a message (android.os.Message instance) to a handler.<br><br>

This event does not occur except for a security level of 0 (lowest).<br><br>

The following child objects are attached to the Event object.<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4erg{border-color:inherit;font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-6t3r{font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-kg9c">Name</th>
    <th class="tg-kg9c">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">what</td>
    <td class="tg-0pky">Represents the type of message.<br>Equivalent to what field of the sent Message instance.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">arg1</td>
    <td class="tg-0lax">An integer value parameter.<br>Equivalent to the arg1 field of the sent Message instance.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">arg2</td>
    <td class="tg-0lax">Integer parameter.<br>Equivalent to the arg2 field of the sent Message instance.</td>
  </tr>
  <tr>
    <td class="tg-0lax">ExternalObject</td>
    <td class="tg-6t3r">obj</td>
    <td class="tg-0lax">Equivalent to the obj field of the sent Message instance.<br>If the value of the obj field is null , an ExternalObject object indicating a null reference will be added.<br>You can check if it is a null reference object by using the <a href="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/extobj/externalobjectjp4.htm" target="_blank" rel="noopener noreferrer">ExternalObject.IsNullRef</a> property.</td>
  </tr>
</tbody>
</table>

<br><small><span style="color:red">Can only be used in AI</span></small><br><small><span style="color:red">Added since AI Ver.1.0.2</span></small>
