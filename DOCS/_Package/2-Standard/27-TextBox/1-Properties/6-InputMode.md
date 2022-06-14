---
layout: default

grand_parent: TextBox Class
parent: Properties
has_children: false
title: InputMode Property
nav_order: 6
permalink: /package/standard/textbox/properties/inputmode
---
# {{ page.title }}

Specify the character types that can be entered.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-34fe{background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">Constant</th>
    <th class="tg-34fe">Value</th>
    <th class="tg-llyw">Description</th>
    <th class="tg-llyw">Character code in UString</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ STD</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">All character types</td>
    <td class="tg-0pky">-</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ NUMERIC</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Half-width numbers, half-width spaces<br>0-9 _ _</td>
    <td class="tg-0pky">U + 0030 to U + 0039</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ ALPHA</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-j5n6">Half-width alphabet, half-width space<br>a ~ z , A ~ Z</td>
    <td class="tg-0pky">U + 0041 ~ U + 005A , U + 0061 ~ U + 007A</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ SYMBOL</td>
    <td class="tg-c3ow">Four</td>
    <td class="tg-0pky">Half-width symbols (half-width numbers, half-width characters other than half-width alphabets), half-width spaces<br>! "# $% &amp;'() = ~ | \ ^-@ []:;, ./ \ _?&gt; &lt;+ * {}`</td>
    <td class="tg-0pky">U + 0021 ~ U + 002F , U + 003A ~ U + 0040 ,<br>U + 005B ~ U + 0060 , U + 007B ~ U + 00FE ,<br>U + F8F0 , U + FF61 ~ U + FF65</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ KANA</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-0pky">Half-width katakana, half-width space<br>A-n</td>
    <td class="tg-0pky">U + FF66 ~ U + FF9F</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DNUMERIC</td>
    <td class="tg-c3ow">16 16</td>
    <td class="tg-0pky">Full-width numbers, full-width / half-width spaces<br>0-9</td>
    <td class="tg-0pky">U + FF10 ~ U + FF19</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DALPHA</td>
    <td class="tg-c3ow">32</td>
    <td class="tg-0pky">Full-width alphabetic characters, full-width / half-width spaces<br>a to z, AZ</td>
    <td class="tg-0pky">U + FF21 ~ U + FF3A , U + FF41 ~ U + FF5A</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DSYMBOL</td>
    <td class="tg-c3ow">64</td>
    <td class="tg-0pky">Full-width symbols (full-width katakana, full-width hiragana, full-width Chinese characters, full-width numbers, full-width characters other than full-width alphabetic characters), full-width / half-width spaces<br>!! "# $% &amp;'() = ~ |` {}<br>* + &lt;&gt;? _ ¥ ・. , "" :; @</td>
    <td class="tg-0pky">Not applicable to others</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DKANA</td>
    <td class="tg-c3ow">128 128</td>
    <td class="tg-0pky">Full-width katakana, full-width / half-width space</td>
    <td class="tg-0pky">U + 30A1 ~ U + 30FA , U + 30FC ~ U + 30FF ,<br>U + 31F0 ~ U + 31FF</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DHIRA</td>
    <td class="tg-c3ow">256</td>
    <td class="tg-0pky">Full-width hiragana, full-width and half-width spaces</td>
    <td class="tg-0pky">U + 3041 ~ U + 3096 , U + 3099 ~ U + 309F</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ DKANJI</td>
    <td class="tg-c3ow">512</td>
    <td class="tg-0pky">Full-width Chinese characters, full-width / half-width spaces</td>
    <td class="tg-0pky">U + 4E00 ~ U + ABFF , U + F900 ~ U + FAFF</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ HANKAKU</td>
    <td class="tg-c3ow">15</td>
    <td class="tg-0pky">Half size</td>
    <td class="tg-0pky">$ NUMERIC , $ ALPHA , $ SYMBOL , $ KANA<br>Applicable to</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ ZENKAKU</td>
    <td class="tg-c3ow">1008</td>
    <td class="tg-0pky">Full-width, full-width / half-width space</td>
    <td class="tg-0pky">$ DNUMERIC , $ DALPHA , $ DSYMBOL , $ DKANA ,<br>Applicable to $ DHIRA and $ DKANJI</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ KANJI</td>
    <td class="tg-c3ow">944</td>
    <td class="tg-0pky">Full-width characters other than full-width symbols, full-width / half-width spaces</td>
    <td class="tg-0pky">$ DNUMERIC , $ DALPHA , $ DKANA , $ DHIRA ,<br>Applicable to $ DKANJI</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ EXSPACE</td>
    <td class="tg-c3ow">0x40000000</td>
    <td class="tg-0pky">This is an option to add to the above specifications. Specify the exclusion of half-width spaces.<br>There is no effect even if it is specified in combination with $ STD or alone.<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add503.gif" alt="Image" width="50" height="12"></td>
    <td class="tg-0pky">Example ) $ DKANA + $ EXSPACE<br>Only full-width katakana and double-byte spaces can be entered</td>
  </tr>
</tbody>
</table>

The function of the OS is used to determine the character type .

Different judgments may be made depending on the OS .

The characters "" may be judged as symbols or Chinese characters by the OS, so be sure to check that they are judged correctly by the OS you actually use.


