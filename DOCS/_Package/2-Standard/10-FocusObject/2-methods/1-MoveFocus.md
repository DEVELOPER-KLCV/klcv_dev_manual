---
layout: default

grand_parent: FocusObject Class
parent: Methods
has_children: false
title: FocusObject.MoveFocus Method
nav_order: 1
permalink: /package/standard/focusobject/methods/movefocus
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">The focus is changed according to the focus movement order.<br><br>Focus may not move correctly in the following cases.<br>-When keyboard focus is set other than the object that called the MoveFocus method.<br>-In the case of an object that is originally in a state where it does not receive focus, such as an option button that has not been selected.<br>-For objects in inactive windows hidden in dialogs.<br><br>Normally, it is used in the <a href="/package/standard/focusobject/events/focusoperation">FocusOperation</a> event of the object whose <a href="/package/standard/focusobject/properties/autotabfocus">AutoTabFocus</a> property is set to $ FALSE. The MoveFocus method is executed only when the OnFocusOperation event handler is used to check the input value for errors and the focus movement is permitted.<br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.2.0.0</span></small><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Constant</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ NEXTFOCUS</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Next object<br>The focus moves in the same order as the Tab key.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ PREVFOCUS</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Previous object<br>The focus moves in the same order as the Shift + Tab keys.</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.MoveFocus( [ <b>direction</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>direction</b></td>
    <td>Direction to move<br>Specify the following values. If omitted, it will be $ NEXTFOCUS<br></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (MessageBox("確認してください", "確認", $OkCancel) == OkSelected) {
    TextBox1.MoveFocus($PREVFOCUS);
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



