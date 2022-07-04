---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.IsPopup Method
nav_order: 3
permalink: /package/extension4/progressbar/methods/ispopup
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Check if it is displayed in a pop-up. <br><br>Pressing the cancel button in the pop-up window closes the window, so you can also use it to find out if the cancel button was pressed.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = pb.IsPopup( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">If it is displayed in a pop-up, $TRUE is returned, otherwise $FALSE is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
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
    <td colspan="2"><a href="/package/extension4/progressbar/methods/popup">Popup</a> method</td>
  </tr>
</table>
