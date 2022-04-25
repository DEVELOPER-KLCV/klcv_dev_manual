---
layout: default

parent: System Functions

title: changeProfile
nav_order: 2
permalink: /method/system/changeProfile
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">In most cases, Biz / Browser can run CRS programs created for previous versions out of the box. However, some functions have been changed or deleted from the specifications due to version transition. <br>Immediately after installation, the function that supports past versions is disabled, but by executing the changeProfile function to switch profiles, some of the changed or deleted specifications can be returned to the conventional specifications. In many cases, switching profiles allows you to run the latest version without changing the program.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">changeProfile (<b>profile</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>	String <b>profile</b></td>
    <td>Specify the profile name to select. <br> If you specify the empty string "", the default settings at the time of installation are restored. You can also specify the following values. <br> The following functions are affected by changing the profile. <br> </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>changeProfile ("4.0.0");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





