---
layout: default

parent: 6. System Functions

title: getPrinterList
nav_order: 11
permalink: /method/system/getPrinterList
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get a list of printers. <br> <small> Not available in mobile and AI.</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">	
var list = getPrinterList( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">List of printers. <br> Returns an array of Record objects with the following child objects:
          <table>
                    <tr>
                        <td>Type</td>
                        <td>Name</td>
                        <td>Explanation</td>
                    </tr>
                    <tr>
                        <td>Number</td>
                        <td><b><i>defaultPrinter</i></b></td>
                        <td>1 for the currently selected printer, 0 for Other</td>
                    </tr>
                    <tr>
                        <td>Number</td>
                        <td><b><i>preview</i></b></td>
                        <td>1 for the dummy printer for preview, 0 for Other</td>
                    </tr>
                    <tr>
                        <td>String</td>
                        <td><b><i>printerName</i></b></td>
                        <td>Printer name</td>
                    </tr>
                    <tr>
                        <td>String</td>
                        <td><b><i>description</i></b></td>
                        <td>Comments set on the printer</td>
                    </tr>
         </table>
    </td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var list = getPrinterList();
for (var n = 0; n < list.Length; n++) {
    print(list[n].defaultPrinter, list[n].preview, list[n].printerName, list[n].description, "\n");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/setDefaultPrinter">setDefaultPrinter</a> function.</td>
  </tr>
</table>





