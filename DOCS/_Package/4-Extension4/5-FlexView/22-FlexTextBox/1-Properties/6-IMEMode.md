---
layout: default

grand_parent: FlexTextBox Class
parent: Properties
has_children: false
title: FlexTextBox.IMEMode Property
nav_order: 6
permalink: /package/extension4/flexview/flextextbox/properties/imemode
---
# {{ page.title }}

If specified, the mode will switch to the specified mode when keyboard focus is received. It also reverts to its previous state when it loses keyboard focus.

In the Mobile version, SIP (Software Input Panel) can also be controlled at the same time.

The operation is undefined when a SIP that does not exist in the model is specified.

<small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>

In addition, an unique SIP control can be performed by combining the Root.<a href="/package/standard/root/methods/setusersip">SetUserSip</a> method with the SIP control plug-in DLL.

<small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>

| Constant | Value | Description                                                                              |
|----------|:-----:|------------------------------------------------------------------------------------------|
| $ STD    |   0   | Do not control IME <br>**_Mobile_** version<br> Ignored when running on Windows Mobile OS        |
| $ ALPHA  |   2   | Half-width Alphanumerical                                                                |
| $ KANA   |   8   | Half-width Katakana                                                                      |
| $ DALPHA |   32  | Full-width Alphanumerical                                                                |
| $ DKANA  |  128  | Full-width Katakana                                                                      |
| $ DHIRA  |  256  | Full-width Hiragana                                                                      |
| $ CLOSE  |  4096 | Close IME <br> **_Mobile_** version <br>Ignored when running on Windows Mobile OS                 |
| $ OPEN   |  8192 | Open IME in default state <br>**_Mobile_** <br>version Ignored when running on Windows Mobile OS |


***Extension in Mobile version***

| Constant       | Value ( hexadecimal ) | Description                                     |
|----------------|:---------------------:|-------------------------------------------------|
| $ SIP_HIRAKATA |        00010000       | Display SIP in "Hiragana / Katakana" mode       |
| $ SIP_ROMAJI   |        00020000       | Display SIP in "Romaji / Kana" mode             |
| $ SIP_KEYBOARD |        00030000       | Show SIP in "keyboard" mode <br><small><span style="color:red">Added since Mobile Ver.3.2.2</span></small>                     |
| $ SIP_HWINPUT  |        00040000       | Display SIP in "Handwriting Input" mode         |
| $ SIP_ENUMBER  |        00050000       | Displays SIP in "alphanumerical" mode  <br><small><span style="color:red">Added since Mobile Ver.3.2.2</span></small>          |
| $ SIP_BUSYU    |        00060000       | Display SIP in "Radical Stroke Search" mode  <br><small><span style="color:red">Added since Mobile Ver.3.2.2</span></small>    |
| $ SIP_SOKAKU   |        00070000       | Display SIP in "Total stroke count search" mode |
| $ SIP_HWSEARCH |        00080000       | Show SIP in "handwriting search" mode           |
| $ SIP_CLOSE    |        10000000       | Hide SIP                                        |
| $ SIP_OPEN     |        20000000       | Displays SIP in the selected mode               |
| $ SIP_USER1    |        000a0000       | For SIP control plug-in assignment    <br><small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>           |
| $ SIP_USER2    |        000b0000       | For SIP control plug-in assignment    <br><small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>          |
| $ SIP_USER3    |        000c0000       | For SIP control plug-in assignment      <br><small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>        |


In addition to the above, the following options can be specified.

| Constant      | Value ( hexadecimal ) | Description                                                                                                                                                   |
|---------------|:---------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| $ SIP_UPPER   |        00100000       | Show SIP at the top of the screen. In this case, the Biz / Browser will not be resized and the SIP will appear to overlap the Biz / Browser .                 |
| $ SIP_AUTOPOS |        00200000       | Displays SIP at the bottom of the screen if the object with focus is at the top of the screen, and $ SIP_UPPER if the object is at the bottom of the screen . |

<br><small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>  

***Restrictions on Mobile version***<br>
When the hardware key is pressed, IME control may not be applied and the character input mode of the hardware key may be prioritized.

***Restrictions on Android version***<br>
In the Android version, IME input mode cannot be controlled due to OS restrictions.

In addition, SIP (Software Input Panel) may not be performed correctly depending on the IME.

The display control of SIP (Software Input Panel) when the value is set in the IMEMode property is as follows.

If you specify a value to display SIP and a value to not display at the same time, SIP will not be displayed.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-0ss8">Action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$ STD</td>
    <td class="tg-j5n6">Do not control</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ CLOSE</td>
    <td class="tg-j5n6" rowspan="2">Do not show SIP</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_CLOSE</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ ALPHA</td>
    <td class="tg-j5n6" rowspan="15">Show SIP</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ KANA</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ DALPHA</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ DKANA</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ DHIRA</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ OPEN</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_HIRAKATA</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_ROMAJI</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_KEYBOARD</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_HWINPUT</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_ENUMBER</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_BUSHU</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_SOKAKU</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_HWSEARCH<br><small><span style="color:red">Added since AI Ver.1.0.1</span></small></td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ SIP_OPEN</td>
  </tr>
</tbody>
</table>

