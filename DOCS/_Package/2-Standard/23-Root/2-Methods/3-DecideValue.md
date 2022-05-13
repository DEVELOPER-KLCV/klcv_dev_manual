---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.DecideValue Property
nav_order: 3
permalink: /package/standard/root/methods/decidevalue
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.DecideValue( )</td>
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
    <td colspan="2">
    <code><pre>
    Form frm1 {
      :
      TextBox tb {
          :
      }
      Function OnClicked(e) {
          //.DecideValue();
          MessageBox("The input value is" + tb.Value );
      }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



