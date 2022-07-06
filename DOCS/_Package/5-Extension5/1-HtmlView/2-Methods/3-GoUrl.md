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
    <td colspan="2">Specify the URL of the web page to display.<br> This method allows to switch the page displayed from the CRS program. <br>Page transition is also possible from the displayed HTML hyperlink.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.GoUrl( <b><i>url</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b><i>url</i></b></td>
    <td>Specifies the URL (URI) string for the page to open.<br> http, ftp, https, file (local path) etc. can be opened.</td>
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