---
layout: default

grand_parent: EditObject Class
parent: Properties
has_children: false
title: EditObject.IMEMode property
nav_order: 10
permalink: /package/standard/editobject/properties/imemode
---
# {{ page.title }}

If specified, the mode will switch to the specified mode when keyboard focus is received. It also reverts to its previous state when it loses keyboard focus.


In the Mobile version, SIP (Software Input Panel) can also be controlled at the same time.

The operation is undefined when a SIP that does not exist in the model is specified.
<br><small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>

You can also perform your own SIP control by combining the Root.SetUserSip method with the SIP control plug-in DLL.
<br><small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>


<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ STD</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Do not control IME<br> <br><span style="font-weight:bold">Mobile version</span><br>Ignored when running on Windows Mobile OS</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ALPHA</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Half-width alphanumerical</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ KANA</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">Half-width Katakana</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DALPHA</td>
    <td class="tg-baqh">32</td>
    <td class="tg-0lax">Full-width alphanumerical</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DKANA</td>
    <td class="tg-baqh">128 128</td>
    <td class="tg-0lax">Full-width katakana</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DHIRA</td>
    <td class="tg-baqh">256</td>
    <td class="tg-0lax">Full-width hiragana</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ CLOSE</td>
    <td class="tg-baqh">4096</td>
    <td class="tg-0lax">Close IME<br> <br><span style="font-weight:bold">Mobile version</span><br>Ignored when running on Windows Mobile OS</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ OPEN</td>
    <td class="tg-baqh">8192</td>
    <td class="tg-0lax">Open IME in default state<br> <br><span style="font-weight:bold">Mobile version</span><br>Ignored when running on Windows Mobile OS</td>
  </tr>
</tbody>
</table>

**Extension in Mobile version**

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value ( hexadecimal )</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ SIP_HIRAKATA</td>
    <td class="tg-baqh">00010000</td>
    <td class="tg-0lax">Display SIP in "Hiragana / Katakana" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_ROMAJI</td>
    <td class="tg-baqh">00020000</td>
    <td class="tg-0lax">Display SIP in "Romaji / Kana" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_KEYBOARD</td>
    <td class="tg-baqh">00030000</td>
    <td class="tg-0lax">Show SIP in "keyboard" mode<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add322.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWINPUT</td>
    <td class="tg-baqh">00040000</td>
    <td class="tg-0lax">Display SIP in "Handwriting Input" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_ENUMBER</td>
    <td class="tg-baqh">00050000</td>
    <td class="tg-0lax">Displays SIP in "alphanumerical" mode<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add322.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_BUSYU</td>
    <td class="tg-baqh">00060000</td>
    <td class="tg-0lax">Display SIP in "Radical Stroke Search" mode <br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add322.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_SOKAKU</td>
    <td class="tg-baqh">00070000</td>
    <td class="tg-0lax">Display SIP in "Total stroke count search" mode <br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add322.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWSEARCH</td>
    <td class="tg-baqh">00080000</td>
    <td class="tg-0lax">Show SIP in "handwriting search" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_CLOSE</td>
    <td class="tg-baqh">10000000</td>
    <td class="tg-0lax">Hide SIP</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_OPEN</td>
    <td class="tg-baqh">20000000</td>
    <td class="tg-0lax">Displays SIP in the selected mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER1</td>
    <td class="tg-baqh">000a0000</td>
    <td class="tg-0lax">For SIP control plug-in assignment<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER2</td>
    <td class="tg-baqh">000b0000</td>
    <td class="tg-0lax">For SIP control plug-in assignment <br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER3</td>
    <td class="tg-baqh">000c0000</td>
    <td class="tg-0lax">For SIP control plug-in assignment<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></td>
  </tr>
</tbody>
</table>

In addition to the above, the following options can be specified.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-23hc">Value ( hexadecimal )</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ SIP_UPPER</td>
    <td class="tg-0lax">00100000</td>
    <td class="tg-0lax">Show SIP at the top of the screen.<br>In this case , the Biz / Browser will not be resized and the SIP will appear to overlap the Biz / Browser .</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_AUTOPOS</td>
    <td class="tg-0lax">00200000</td>
    <td class="tg-0lax">Displays SIP at the bottom of the screen if the object with focus is at the top of the screen, and $ SIP_UPPER if the object is at the bottom of the screen .</td>
  </tr>
</tbody>
</table>

<br><small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>

**Restrictions on Mobile version**<br>
When the hardware key is pressed, IME control may not be applied and the character input mode of the hardware key may be prioritized.

**Restrictions on Android version**<br>
In the Android version, IME input mode cannot be controlled due to OS restrictions .

Also, depending on the IME , SIP (Software Input Panel) may not be performed correctly.

 

The display control of SIP (Software Input Panel) when the value is set in the IMEMode property is as follows.

If you specify a value that displays SIP and a value that does not display SIP at the same time, SIP will not be displayed.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-23hc">Operation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ STD</td>
    <td class="tg-0lax">Do not control</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ CLOSE</td>
    <td class="tg-0lax" rowspan="2">Hide SIP</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_CLOSE</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ ALPHA</td>
    <td class="tg-0lax" rowspan="15">Show SIP</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ KANA</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DALPHA</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DKANA</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ DHIRA</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ OPEN</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HIRAKATA</td>
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
    <td class="tg-0lax">$ SIP_BUSHU</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_SOKAKU</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWSEARCH<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add101.gif" alt="Image" width="65" height="12"></td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_OPEN</td>
  </tr>
</tbody>
</table>








