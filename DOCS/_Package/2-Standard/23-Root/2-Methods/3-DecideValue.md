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
    <td colspan="2">Forced to confirmed the value of an object whose input is unconfirmed.<br><br>Derived classes of the <a href="/package/standard/editobject">EditObject</a> class determine the value you are typing when keyboard focus is lost or when you press the Enter or Function key. Prior to that, the value entered on the screen will not be set in the Value property and will be in an undetermined state.<br><br>The DecideValue method forces the value of such an undetermined object to the Value property.Used when handling input values in event handlers that do not involve input confirmation behavior, such as the Label object's Clicked and Timer events.<br><br>By calling the DecideValue method, events related to value changes such as Touch event and Change event may occur.</td>
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



