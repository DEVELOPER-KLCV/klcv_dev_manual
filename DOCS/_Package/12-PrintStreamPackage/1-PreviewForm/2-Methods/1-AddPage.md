---
layout: default

grand_parent: PreviewForm Class
parent: Methods
has_children: false
title: PreviewForm.AddPage Method
nav_order: 1
permalink: /package/printstreampackage/previewform/methods/addpage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">preview.AddPage( <b>page</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>page</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PSS-10</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var count = PrintStreamDocument1.GetPageCount();
    StartPage(PrintStreamDocument1);
    for (var page = 1; page <= count; page++) {
        AddPage(page);
    }
    EndPage();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/printstreampackage/previewform/methods/startpage">StartPage</a>, <a href="/package/printstreampackage/previewform/methods/endpage">EndPage</a> methods</td>
  </tr>
</table>



