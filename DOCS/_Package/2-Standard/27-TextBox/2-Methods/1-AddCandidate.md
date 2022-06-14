---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: TextBox.AddCandidate Method
nav_order: 1
permalink: /package/standard/textbox/methods/addcandidate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add to the candidate list in the text box.<br>Character strings entered with text completion are not subject to input restrictions due to the setting of the <a href="/base/inputmode">InputMode</a> property. Specifying the <a href="/package/standard/editbox/properties/maxlength">MaxLength</a> property is valid, but the <a href="/package/standard/editbox/properties/maxlengthreached">MaxLengthReached</a> event does not occur. Also, the  <a href="/package/standard/editbox/properties/autotab">AutoTab</a> property setting is ignored.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TextBox1.AddCandidate( <b><i>suggest</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>suggest</i></b></td>
    <td>Character string displayed in the candidate</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TextBox1.AddCandidate("Candidate");
    TextBox1.AddCandidate("Candidate List");
    </pre></code></td> 
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/textbox/methods/clearcandidate">ClearCandidate</a> method</td>
  </tr>
</table>



