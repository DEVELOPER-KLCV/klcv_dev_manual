---
layout: default

grand_parent: HtmlView Class
parent: Methods
has_children: false
title: HtmlView.GoUrl Method
nav_order: 3
permalink: /package/extension5/htmlview/methods/gourl
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.GoUrl( <b>url</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>url</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Button b {
        X = 8;
        Y = 8;
        Width = 95;
        Height = 70;
        Function OnTouch(e) {
            ^.HtmlView1.GoUrl("http://google.co.jp/");
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>