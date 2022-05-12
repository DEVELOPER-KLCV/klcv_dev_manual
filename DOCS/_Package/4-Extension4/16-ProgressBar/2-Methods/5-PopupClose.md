---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.PopupClose Method
nav_order: 5
permalink: /package/extension4/progressbar/methods/popupclose
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">pb.PopupClose( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
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