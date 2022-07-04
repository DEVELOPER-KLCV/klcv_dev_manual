---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.AutoStep Method
nav_order: 1
permalink: /package/extension4/progressbar/methods/autostep
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Starts the automatic progress of the progress bar. <br><br>It is used when you want to automatically advance steps at regular intervals without advancing steps with the <a href="/package/extension4/maskedit/methods/stepit">StepIt</a> method.<br> For <b><i>sec</i></b>, specify the time until the step reaches the maximum value specified by the <a href="/package/extension4/progressbar/properties/step">Step</a> property.<br> For example, if the Step property is 10, if you specify 1 (second), it will advance 10 steps per second.<br><br> Calling the a href="/package/extension4/maskedit/methods/autostepoff">AutoStepOff</a> method will stop auto-progress.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ProgressBar1.AutoStep( <b><i>sec</i></b> [, <b><i>flag</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b><i>sec</i></b></td>
    <td>Time (seconds) until the step reaches the maximum value<br> It can be specified in 0.1 second increments. Make sure that one step does not take less than 0.1 seconds.</td>
  </tr>
  <tr>
    <td>boolean  <b><i>flag</i></b></td>
    <td>If $TRUE is specified, the ><a href="/package/extension4/progressbar/events/timer">Timer</a> event will be generated for each step.</td>
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
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/progressbar/properties/step">Step</a> property<br><a href="/package/extension4/maskedit/methods/autostepoff">AutoStepOff</a>, <a href="/package/extension4/maskedit/methods/stepit">StepIt</a> methods<br><a href="/package/extension4/progressbar/events/timer">Timer</a> event</td>
  </tr>
</table>