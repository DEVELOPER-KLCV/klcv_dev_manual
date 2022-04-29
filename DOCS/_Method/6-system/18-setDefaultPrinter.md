---
layout: default

parent: 6. System Functions

title: setDefaultPrinter
nav_order: 18
permalink: /method/system/setDefaultPrinter
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the default printer. This setting is not related to the default printer of Windows and changes the setting inside Biz / Browser. <br> If you print without specifying the printer name in the Doc object, it will be printed to the printer specified by the setDefaultPrinter function. <br> Immediately after starting Biz / Browser, the default printer for Windows is selected. <br> <small>Not available in Mobile and AI </small> </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">setDefaultPrinter (<b>printer</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>printer</b></td>
    <td>Specify the printer name to select. <br><br> If "[preview]" is specified, the preview printer will be selected. <br> If null is specified, the Windows default printer will be selected. <br><br> Otherwise, the  <b>printer</b> with the same name as printer will be selected. If no matching printer is found, the selection status does not change.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>setDefaultPrinter("[preview]");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/getPrinterList">getPrinterList</a> function.</td>
  </tr>
</table>





