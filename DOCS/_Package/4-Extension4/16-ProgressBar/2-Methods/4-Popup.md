---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.Popup Method
nav_order: 4
permalink: /package/extension4/progressbar/methods/popup
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">The progress bar will pop up in a separate window.<br> Only ProgressBar objects created with the <a href="/package/extension4/progressbar/methods/create">Create</a> method can be used.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">pb.Popup( [ <b><i>UseCancel</i></b> [, <b><i>UseMessage</i></b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>boolean <b><i>UseCancel</i></b></td>
    <td>If $TRUE is specified, a cancel button will be displayed. <br>Use the <a href="/package/extension4/progressbar/methods/ispopup">IsPopup</a> method to check if it was canceled.</td>
  </tr>
  <tr>
    <td>boolean <b><i>UseMessage</i></b></td>
    <td>If $TRUE is specified, the message string specified by the <a href="/package/extension4/progressbar/properties/message">Message</a> property will be displayed.<br><small><span style="color:red">Added since Ver.5.0.0</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var pb = ProgressBar.Create();
    pb.Width = 200;
    pb.Height = 20;
    pb.Step = 10;
    pb.Title = "Loading";
    pb.Popup($TRUE);
    for (var i = 0; i < 10; i++) {
        ...
        if (!pb.IsPopup()) {
            break;
        }
        pb.StepIt();
    }
    pb.PopupClose();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/progressbar/properties/message">Message</a> property<br><a href="/package/extension4/progressbar/methods/create">Create</a>, <a href="/package/extension4/progressbar/methods/ispopup">IsPopup</a> methods</td>
  </tr>
</table>