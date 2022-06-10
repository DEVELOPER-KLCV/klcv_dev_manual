---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: Spread.SetEditor Method
nav_order: 7
permalink: /package/standard/spread/methods/seteditor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Paste the specified object into the cell being edited.<br><br>The object is not always displayed, it is displayed only at the cell position when the SetEditor method is executed, and when the cursor moves, the <a href="/package/standard/spread/events/stopedit">StopEdit</a> event is fired and released.<br><br>Make sure to execute the SetEditor method from within the event handler of the <a href="/package/standard/spread/events/startedit">StartEdit</a> event. It is possible to call SetEditor at other times, but it will be easier to control if it is processed by the StartEdit and StopEdit events.</td>
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
    <td>Object <b><i>obj</i></b></td>
    <td>Specify the object you want to paste for editing.<br>If obj is not specified, the current setting will be canceled.</td>
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



