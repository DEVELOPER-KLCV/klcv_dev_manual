---
layout: default

grand_parent: ProgressBar Class
parent: Methods
has_children: false
title: ProgressBar.StepIt Method
nav_order: 6
permalink: /package/extension4/progressbar/methods/stepit
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Take the progress bar one step.<br> If specify an argument, the progress bar advances to the step position of that numerical value.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var num = ProgressBar1.StepIt( [ <b><i>num</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>num</i></b></td>
    <td>Step position<br>Specify a value less than or equal to <a href="/package/extension4/progressbar/properties/step">Step</a> property. If omitted, proceed one step.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function func() {
        func1();
        ProgressBar1.StepIt();
        func2();
        ProgressBar1.StepIt();
        func3();
        ProgressBar1.StepIt();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/progressbar/properties/step">Step</a> property</td>
  </tr>
</table>
