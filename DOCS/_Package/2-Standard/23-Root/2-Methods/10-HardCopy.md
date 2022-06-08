---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.HardCopy Property
nav_order: 10
permalink: /package/standard/root/methods/hardcopy
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Output a hard copy (screen capture) of the screen to the printer.<br><br>In addition to the screen image, supplementary information for hard copy printing can be added. <br>Hardcopy is always printed from the printer. It cannot be output to the preview screen or image file.<br><small><span style="color:red">Added since Ver.4.0.0</span></small><br><br>You can get a hardcopy as an Image object instead of printing by specifying a special virtual printer for the printer name.<br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.HardCopy( [ <b>mode</b> [ , <b>option</b> [ , <b>comment</b> [ , <b>printer</b> ] ] ] ] )<br>OR</br>var img = //.HardCopy( <b>mode</b>, 0, “”, “@image” )<br><small><span style="color:red">Added since Ver.5.0.3</span></small>
 </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>mode</b></td>
    <td>Select the print target from the following.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-e0s6{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-wb7o{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-wb7o">Constant</th>
    <th class="tg-e0s6">Value</th>
    <th class="tg-wb7o">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$ HC_FORM</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">Print the Form object of the Root object .<br>Window frames and title bars are not printed.</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ HC_WINDOW</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Print the Biz / Browser window as it is.<br>Window borders and titles are also printed.<br>If it is running in Internet Explorer , it will behave the same as $ HC_FORM .</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ HC_DESKTOP</td>
    <td class="tg-tcrt">2</td>
    <td class="tg-i7zr">Prints the entire desktop.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ HC_DIALOG</td>
    <td class="tg-tcrt">3</td>
    <td class="tg-i7zr">Prints the single dialog at the top.<br>The behavior is undefined when the dialog is not displayed.<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add500.gif" alt="Image" width="50" height="12"><br>Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"><br></td>
  </tr>
</tbody>
</table><br>If mode is omitted, the operation will be $ HC_FORM.</td>
  </tr>
  <tr>
    <td>integer <b>option</b></td>
    <td>Specify the supplementary information to be included in the print in the following combination. <br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-e0s6{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-wb7o{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-wb7o">Constant</th>
    <th class="tg-e0s6">Value</th>
    <th class="tg-wb7o">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">HC_VERSION</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Print the version information of Biz / Browser .</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ HC_INFO</td>
    <td class="tg-lcf4">2</td>
    <td class="tg-j5n6">Print the Windows version and computer name.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ HC_DATE</td>
    <td class="tg-tcrt">4</td>
    <td class="tg-i7zr">Print the current date and time.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ HC_COMMENT</td>
    <td class="tg-tcrt">8</td>
    <td class="tg-i7zr">Print the comment. The comment body is specified by comment .<br>If you do not specify $ HC_COMMENT, the comment will not be printed.</td>
  </tr>
</tbody>
</table><br><br>Also, select the orientation of the paper to print from the following.<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-e0s6{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-wb7o{background-color:#D9D9D9;border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-wb7o">Constant</th>
    <th class="tg-e0s6">Value</th>
    <th class="tg-wb7o">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$ HC_VERTICAL</td>
    <td class="tg-j5n6">256</td>
    <td class="tg-j5n6">Print vertically</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ HC_HORIZONTAL</td>
    <td class="tg-j5n6">512</td>
    <td class="tg-j5n6">Print horizontally</td>
  </tr>
</tbody>
</table><br>If you do not specify the paper orientation, it will be the default orientation of the printer.<br><br>If you omit the <b><i>option</i></b> or specify 0, no supplemental information is printed and the paper orientation is the printer's default orientation.<br><br>When specifying multiple supplementary information, add and specify as follows. <br>
    <code><pre>
    //.HardCopy($HC_a </pre></code></td>
  </tr>
  <tr>
    <td>String <b>comment</b></td>
    <td>Specify the comment to be printed as a supplement to the hard copy. <br>This is valid only when $ HC_COMMENT is specified for  <b><i>option</i></b>.</td>
  </tr>
  <tr>
    <td>String <b>printer</b></td>
    <td>Specify the output destination printer name. The printer name can be obtained with the <a href="/method/system/getPrinterList">getPrinterList</a> function.<br><br>If a blank character string or null is specified for <b><i>printer</i></b>, the printer selection dialog is displayed. The user can select any printer.<br><br>If <b><i>printer</i></b> is omitted, it will be output to the normally used printer set in Biz / Browser. The default printer for Biz / Browser is set with the <a href="/method/system/setDefaultPrinter">setDefaultPrinter</a> function. <br><br><small><span style="color:green">The following parameters can be specified since Ver.5.0.3</span></small><br>By specifying "@image" as a special printer name, the result of hard copy can be obtained as an Image object by the return value of the method.</td>
  </tr>
  <tr>
    <td rowspan="6">Exception</td>
    <td>PKG-39</td>
    <td>Cannot output to preview printer</td>
  </tr>
  <tr>
    <td>PKG-40</td>
    <td>Ended error</td>
  </tr>
  <tr>
    <td>PKG-41</td>
    <td>Printer not found</td>
  </tr>
  <tr>
    <td>PKG-42</td>
    <td>The printer could not be opened</td>
  </tr>
  <tr>
    <td>PKG-43</td>
    <td>Could not start printer job</td>
  </tr>
  <tr>
    <td>PKG-44</td>
    <td>Insufficient memory</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.HardCopy($HC_FORM, $HC_VERSION + $HC_COMMENT, "TEST", null);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



