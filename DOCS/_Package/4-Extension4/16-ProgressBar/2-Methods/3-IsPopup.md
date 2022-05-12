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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = pb.IsPopup( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
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
    <td colspan="2"><a href="/package/extension4/progressbar/properties/popup">Popup</a> method</td>
  </tr>
</table>
