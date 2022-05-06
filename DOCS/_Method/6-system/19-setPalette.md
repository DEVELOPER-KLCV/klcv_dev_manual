---
layout: default

parent: 6. System Functions

title: setPalette
nav_order: 19
permalink: /method/system/setPalette
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Change the color of the [color constant]().</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">setPalette(<b>color, R, G, B</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Argument</td>
    <td>integer <b><i>color</i></b> </td>
    <td>	Specify the 0-based color number you want to change. <br> Specify $ RED-1 to change the color of $ RED. <br>able to specify between 0 to 115.</td>
  </tr>
  <tr>
    <td>integer <b><i>R</i></b> </td>
    <td>	Specifies the red intensity of the new color in the range 0-255.</td>
  </tr>
  <tr>
    <td>integer <b><i>G</i></b> </td>
    <td>	Specifies the green intensity of the new color in the range 0-255.</td>
  </tr>
  <tr>
    <td>integer <b><i>B</i></b> </td>
    <td>	Specifies the blue intensity of the new color in the range 0-255.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre> setPalette (8, 128, 128, 255);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





