---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.MessageBox Method
nav_order: 1
permalink: /package/standard/displayobject/methods/Messagebox
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.MessageBox( <b>message</b> [, <b>title</b> [, <b>flag</b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>message</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>title</b></td>
    <td></td>
  </tr>
  <tr>
    <td>intger <b>flag</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (MessageBox("確認してください", "確認", $OKCANCEL) == OkSelected) {
    :
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/displayobject/events/OkSelected">OkSelected</a>, <a href="/package/standard/displayobject/events/CancelSelected">CancelSelected</a>, <a href="/package/standard/displayobject/events/YesSelected">YesSelected</a>, <a href="/package/standard/displayobject/events/NoSelected">NoSelected</a>, <a href="/package/standard/displayobject/events/RetrySelected">RetrySelected</a> events</td>
  </tr>
</table>