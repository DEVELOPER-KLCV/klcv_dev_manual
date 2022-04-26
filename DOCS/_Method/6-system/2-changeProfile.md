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
    <td>Specify the profile name to select. <br> If you specify the empty string "", the default settings at the time of installation are restored. You can also specify the following values. <br> The following functions are affected by changing the profile. <br> 
    <table>
      <tr>
        <td rowspan="2">Function</td>
        <td colspan="4">Profile</td>
      </tr>
      <tr>
        <td>3.0.0</td>
        <td>3.1.0</td>
        <td>4.0.0</td>
        <td>4.1.0</td>
      </tr>
      <tr>
        <td>Background color at startup</td>
        <td>Light blue</td>
        <td>Light blue</td>
        <td>Dark blue</td>
        <td>Gray</td>
      </tr>
      <tr>
        <td>Use of CatchEvent and PeekEvent statements</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Use of Event and From symbols in event handlers</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Substitution of class name for ver2.0 (Replace Record which is a child of Spread with SpreadRow, etc.)</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Ability to reference the Object.className property as an Object.class</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Using the index property of the array definition object</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Using the length property of an array element object</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Invalid</td>
        <td>Invalid</td>
      </tr>
      <tr>
        <td>Enable Vertical Align of Label on the screen</td>
        <td>Invalid</td>
        <td>Valid</td>
        <td>Valid</td>
        <td>Valid</td>
      </tr>
      <tr>
        <td>Ability to raise an exception when Spread.value is set to a value greater than the actual number of rows</td>
        <td>Invalid</td>
        <td>Invalid</td>
        <td>Valid</td>
        <td>Valid</td>
      </tr>
      <tr>
        <td>A function that raises an exception when a value other than the specifiable value is set for Spread.ColumnPosition</td>
        <td>Invalid</td>
        <td>Invalid</td>
        <td>Valid</td>
        <td>Valid</td>
      </tr>
      <tr>
        <td>Ability to raise an exception when setting values ​​for TabFrom.Width and TabForm.Height</td>
        <td>Invalid</td>
        <td>Invalid</td>
        <td>Valid</td>
        <td>Valid</td>
      </tr>
    </table>
    <br>
    Also, from ver4.0.6, the following functions have been affected in order to improve compatibility when printing with ver3.0. When changeProfile ("3.0.0") or changeProfile ("3.1.0") is executed, the print result will be close to ver3.x. However, it does not affect the print result of the <a href="">PrintStream package</a>.<br>In the form printing of ver3.x, the line feed position may change due to the fluctuation of the character spacing depending on the printer and preview environment due to the problem of internal accuracy, but this problem is also solved in ver4.0 by specifying changeProfile. It works in the same way as ver3.x including it (printing accuracy is reduced). When the form printing of ver4.0 and the form printing of ver3.x are mixed, please be careful to switch the profile appropriately.<br><br>

    <table>
      <tr>
        <td rowspan="2">Function</td>
        <td colspan="4">Profile</td>
      </tr> 
      <tr>
        <td>3.0.0</td>
        <td>3.1.0</td>
        <td>4.0.0</td>
        <td>4.1.0</td>
      </tr>
      <tr>
        <td>Internal accuracy of font size</td>
        <td>integer</td>
        <td>integer</td>
        <td>Floating point</td>
        <td>Floating point</td>
      </tr>
      <tr>
        <td>Reference resolution used to calculate the layout of the character string</td>
        <td>90 DPI</td>
        <td>90 DPI</td>
        <td>96 DPI</td>
        <td>96 DPI</td>
      </tr>
    </table>
    If you specify a character string other than the above for profile, the profile will not be changed.
    </td>
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





