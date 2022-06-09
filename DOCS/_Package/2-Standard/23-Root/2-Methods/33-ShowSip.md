---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.ShowSIP Property
nav_order: 33
permalink: /package/standard/root/methods/showsip
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Controls the display of SIP (Software Input Panel). <br><small><span style="color:red">Added since Ver.5.1.0, Mobile Ver.3.1.0, AI Ver.1.0.0</span></small><br><br>Also, in the Mobile version, it is possible to perform original SIP control by combining the SetUserSip method with the SIP control plug-in DLL. <br><small><span style="color:red">Added since Ver.4.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.ShowSIP( <b><i>type</i></b>, <b><i>initial</i></b> )<br><br><b><i>Mobile, Android version</i></b><br>//.ShowSIP( <b><i>mode</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Value selected by SIP<br><br> <b><i>Mobile version, Android version</i></b><br> None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>type</i></b></td>
    <td>Specify one of the following values.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c9ql{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c9ql">Constant</th>
    <th class="tg-7jy7">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">0</td>
    <td class="tg-f8tv">Pops up the calculator directly under the current focus object</td>
  </tr>
  <tr>
    <td class="tg-c3ow">1</td>
    <td class="tg-f8tv">Pops up a calendar directly under the current focus object</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Any <b><i>initial</i></b></td>
    <td>Specify the initial value of SIP. The required type differs depending on the type.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c9ql{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c9ql">Type</th>
    <th class="tg-7jy7">Value</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">0</td>
    <td class="tg-f8tv">Number type</td>
  </tr>
  <tr>
    <td class="tg-c3ow">1</td>
    <td class="tg-f8tv">Date type</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>integer <b><i>mode</i></b></td>
    <td><b><i>Mobile version</i></b><br>Specify one of the following values.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c9ql{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c9ql">Constant</th>
    <th class="tg-7jy7">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">$ SIP_HIRAKATA</td>
    <td class="tg-f8tv">Display SIP in "Hiragana / Katakana" mode</td>
  </tr>
  <tr>
    <td class="tg-c3ow">$ SIP_ROMAJI</td>
    <td class="tg-f8tv">Display SIP in "Romaji / Kana" mode</td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_HWINPUT</td>
    <td class="tg-0lax">Display SIP in "Handwriting Input" mode</td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_HWSEARCH</td>
    <td class="tg-0lax">Show SIP in "handwriting search" mode</td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_CLOSE</td>
    <td class="tg-0lax">Hide SIP</td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_OPEN</td>
    <td class="tg-0lax">Displays SIP in the selected mode</td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_USER1</td>
    <td class="tg-0lax">For SIP control plug-in assignment<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_USER2</td>
    <td class="tg-0lax">For SIP control plug-in assignment<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-baqh">$ SIP_USER3</td>
    <td class="tg-0lax">For SIP control plug-in assignment<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
</tbody>
</table>
<br>In addition to the above, the following options can be specified.<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7jy7">constant</th>
    <th class="tg-7jy7">explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ SIP_UPPER</td>
    <td class="tg-f8tv">Show SIP at the top of the screen.<br>In this case, the Biz / Browser will not be resized and the SIP will appear to overlap the Biz / Browser.</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ SIP_AUTOPOS</td>
    <td class="tg-f8tv">Displays SIP at the bottom of the screen if the object with focus is at the top of the screen, and $ SIP_UPPER if the object is at the bottom of the screen.</td>
  </tr>
</tbody>
</table>
<b><i>Android version</i></b><br>
In the Android version, it is not possible to control the SIP input mode due to OS restrictions.<br>

Also, depending on the IME application, SIP may not be controlled correctly.<br><br>

The SIP display control when a value is set in the ShowSIP method is as follows.<br>

If specify a value to display SIP and a value to not display at the same time, SIP will not be displayed.<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7jy7">Constant</th>
    <th class="tg-7jy7">Action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ SIP_CLOSE</td>
    <td class="tg-f8tv">Do not show SIP</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ SIP_HIRAKATA</td>
    <td class="tg-f8tv" rowspan="10">Show SIP</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_ROMAJI</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_KEYBOARD</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWINPUT</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_ENUMBER</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_BUSYU</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_SOKAKU</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWSEARCH<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add101.gif" alt="Image" width="65" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_CLOSE</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_OPEN</td>
  </tr>
</tbody>
</table>

</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.ShowSIP($SIP_HWINPUT + $SIP_AUTOPOS);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/setusersip">SetUserSip</a> method</td>
  </tr>
</table>



