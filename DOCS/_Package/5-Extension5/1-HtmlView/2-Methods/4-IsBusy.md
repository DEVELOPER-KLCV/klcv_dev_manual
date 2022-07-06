---
layout: default

grand_parent: HtmlView Class
parent: Methods
has_children: false
title: HtmlView.IsBusy Method
nav_order: 4
permalink: /package/extension5/htmlview/methods/isbusy
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns whether the current state is page loading.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.IsBusy( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns $TRUE if the state is loading a page, $FALSE otherwise.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-27</td>
    <td>Initialization has not been completed</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (^.HtmlView1.IsBusy() == $TRUE) {
        ^.HtmlView.Stop();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>