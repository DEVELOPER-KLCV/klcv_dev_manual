---
layout: default

grand_parent: Doc Class
parent: Methods
has_children: false
title: Doc.ShowPage Method
nav_order: 3
permalink: /package/standard/doc/methods/showpage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Breaks the page and sends the page to the printer.<br><br>For a one -page document, a call to the ShowPage method prints that page. Nothing is printed unless you call the ShowPage method.<br><br>For multi-page documents, all but the last page will be printed automatically, but the last page will not be printed unless you call the ShowPage method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Doc1.ShowPage( )</td>
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
Doc Doc1 {
    Format = "A4H";
    Form Form1 {
        Width = 400;
        Height = 400;
        Label Label1 {
            Width = 80;
            Height = 30;
            Border = $TRUE;
        }
    }
    ShowPage();
    Delete();
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>