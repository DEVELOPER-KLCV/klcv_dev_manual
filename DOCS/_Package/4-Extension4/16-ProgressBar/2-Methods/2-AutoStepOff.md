---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.AutoStepOff Method
nav_order: 2
permalink: /package/extension4/progressbar/methods/autostepoff
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Stops the automatic progress of the progress bar started by the <a href="/package/extension4/progressbar/methods/autostep">AutoStep</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ProgressBar1.AutoStepOff( )</td>
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
    ProgressBar1.Step = 10;
    ProgressBar1.AutoStep(5);
    ...
    if (...) {
        ProgressBar1.AutoStepOff();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/progressbar/methods/autostep">AutoStep</a> method</td>
  </tr>
</table>