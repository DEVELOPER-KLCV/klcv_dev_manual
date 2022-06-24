---
layout: default

grand_parent: FlexView Class
parent: Methods
has_children: false
title: FlexView.IndentSort Method
nav_order: 5
permalink: /package/extension4/flexview/flexview/methods/indentsort
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sort the FlexIndentLabel column so that indents can connect.<br><br>The FlexIndentLabel column can express the parent-child relationship by the key property and ParentKey property of FlexIndentLabelCell, and indent the parent and child placed in consecutive rows, but the IndentSort method indents as many rows as possible. Sort the contents of the Key and ParentKey properties by key so that they can be viewed.<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><br><small><span style="color:red">Additional function since Ver.4.1.3 ---> </span></small>col, ad, and prop arguments can now be specified. If col or later is specified, sorting will be performed according to the specified conditions before the indent connection.<small><span style="color:red"> <--- Until here</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">FlexView1.IndentSort( [ <b><i>col</i></b> [, <b><i>arr</i></b>[, <b><i>prop</i></b> ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>col</i></b></td>
    <td>Specifies the number of columns to sort</td>
  </tr>
    <tr>
    <td>String <b><i>arr</i></b></td>
    <td>Specify the sort direction.<br> If "d" is specified, it will be sorted in descending order.<br> Otherwise, sort in ascending order.</td>
  </tr>
    <tr>
    <td>String <b><i>prop</i></b></td>
    <td>Specify the property to be used as the sort key as a string. If omitted, the operation is the same as when "value" is specified.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-6</td>
    <td>FlexRecord not found</td>
  </tr>
    <tr>
    <td>EXT-14</td>
    <td>Column not found</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    FlexView1.IndentSort();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>