---
layout: default

parent: 6. System Functions

title: decodeURL
nav_order: 5
permalink: /method/system/decodeURL
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Decodes URL - encoded strings</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = decodeURL (<b>str</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the decoded string.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>str</b></td>
    <td>Specify the character string to decode.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var url = decodeURL ("http: // server / app1? name =% 83% 41% 83% 4e% 83% 56% 83% 58 & value = Browser% 26Designer");
print (url, "\ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/encodeURL">encodeURL</a> function</td>
  </tr>
</table>





