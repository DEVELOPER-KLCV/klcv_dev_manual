---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: Spread.SetEditor Property
nav_order: 7
permalink: /package/standard/spread/methods/seteditor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Spread1.SetEditor( [ <b>obj</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b>obj</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    Number e_row = -1;
    Number e_col = -1;
    Function OnStartEdit(e) {
        if (e.col == 0){
            SetEditor(SpreadForm.TextBox1);
            SpreadForm.TextBox1.SetFocus();
            SpreadForm.TextBox1.Visible = $TRUE;
            e_row = e.row;
            e_col = e.col;
        }
    }
    
    Function OnStopEdit(e){
        if (e.col == e_col && e.row == e_row) {
            Row[e.row].col0 = SpreadForm.TextBox1;
            SpreadForm.TextBox1.Visible = $FALSE;
            e_row = -1;
            e_col = -1;
        }
    }
    </pre></code>
    In the above example, the TextBox object that is hidden and created elsewhere is pasted in the StartEdit event and released in the StopEdit event. This allows you to enter cells.
    </td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/spread/events/startedit">StartEdit</a>, <a href="/package/standard/spread/events/stopedit">StopEdit</a> events</td>
  </tr>
</table>



