---
layout: default

grand_parent: HtmlView Class
parent: Methods
has_children: false
title: HtmlView.GoForward Method
nav_order: 2
permalink: /package/extension5/htmlview/methods/goforward
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Moves the currently displayed page to the next page. <br>It can be used when the page is changed by the <a href="/package/extension5/htmlview/methods/goback">GoBack</a> method.<br> Page transitions from the <a href="/package/extension5/htmlview/methods/gourl">GoURL</a> method and hyperlinks do not allow page transitions with the GoForward method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.GoForward( )</td>
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
    ^.HtmlView1.GoForward();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/htmlview/methods/goback">GoBack</a> method</td>
  </tr>
</table>