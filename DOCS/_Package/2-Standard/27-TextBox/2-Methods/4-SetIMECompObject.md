---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: TextBox.SetIMECompObject Method
nav_order: 4
permalink: /package/standard/textbox/methods/setimecompobject
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">A method for specifying a TextBox object that receives IME input and using the key input passed to IME. With this method, it is possible to identify the ruby of kanji.<br><br>Executes a method from a TextBox (or its derived class) object that receives IME input and automatically fills another TextBox object in the specified display format.<br><br>Input to the auto-filled object follows IME input. Even if it is converted to alphabetic characters, it will be entered exactly as you entered the key. (Example: "aiu"-> "アイウ") To input alphabets, it is necessary to disable IME of the IME input object.<br><br>Editing on the input character string after the IME input is confirmed is not reflected in the auto-input target object. The new IME input after confirmation is additionally input to the object to be automatically input. If the IME input object is cleared, the auto-input target object is also cleared.<br><br>When a Touch event occurs on an IME input object, the Touch event also occurs on the object to be automatically input.<br><br>Autofill is controlled by the properties of the IME input object as follows:<br>
     1. If the Format property is specified, autofill will also be displayed in the format according to that Format property.<br>
     2. The InputMode and MaxLength properties are valid. The following is an example when IME is entered as "東京都豊島区東池袋１－２３－４".
   <br>

  <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">InputMode</th>
    <th class="tg-llyw">MaxLength</th>
    <th class="tg-llyw">Conversion input </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ DKANA</td>
    <td class="tg-0pky">Unspecified </td>
    <td class="tg-0pky">トウキョウトトシマクヒガシイケブクロ</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DKANA + $ DNUMERIC</td>
    <td class="tg-0pky">Unspecified </td>
    <td class="tg-0pky">トウキョウトトシマクヒガシイケブクロ１２３４</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DKANA</td>
    <td class="tg-0pky">10</td>
    <td class="tg-0pky">トウキョウ</td>
  </tr>
</tbody>
</table>

<small><span style="color:red">Added since Ver.4.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

   </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TextBox1.SetIMECompObject( <b><i>obj</i></b> [, <b><i>mode</i></b> [, <b><i>showRealtime</i></b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>TextBox <b><i>obj</i></b></td>
    <td>TextBox object for auto-input<br>You can specify a TextBox (or its derived class). If null is specified, the setting will be canceled.</td>
  </tr>
  <tr>
    <td>integer <b><i>mode</i></b></td>
    <td>Display format<br>$ KANA: Half-width Katakana <br> $ DKANA: Full-width Katakana <br> $ DHIRA: Full-width Hiragana<br>The default is $ DKANA. Key input such as numbers and symbols is not omitted.</td>
  </tr>
  <tr>
    <td>boolean <b><i>showRealtime</i></b></td>
    <td>Real-time execution control of auto-input<br>$ FALSE: Convert only when IME is confirmed <br>$ TRUE: IME input is automatically input in real time</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-54</td>
    <td>No valid TextBox object specified</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TextBox TextBoxShow {  /* 自動入力用 */
        X = 8;
        Y = 140;
        Width = 136;
        Height = 24;
    }
    TextBox TextBox1 {  /* IME入力用 */
        X = 8;
        Y = 40;
        Width = 136;
        Height = 24;
        IMEMode = $DHIRA;
        SetIMECompObject(^.TextBoxShow, $DKANA, $TRUE);
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



