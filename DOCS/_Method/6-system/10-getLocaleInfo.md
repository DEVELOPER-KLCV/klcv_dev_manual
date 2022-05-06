---
layout: default

parent: 6. System Functions

title: getLocaleInfo
nav_order: 10
permalink: /method/system/getLocaleInfo
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets locale-specific information. <br> <small> Added since Ver.4.1.0.</small><br><small>Not available in Mobile and AI.</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">	
var info = getLocaleInfo (<b>id</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the information corresponding to <b>id</b> as a number or string.<br>If the information corresponding to <b>id</b> is not found, null is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>id</b>&nbsp;&nbsp;&nbsp; &nbsp;   Specify the ID of the information to be acquired from the following.
        <table>
                    <tr>
                        <td>Value</td>
                        <td>Explanation</td>
                    </tr>
                    <tr>
                        <td>"encoding"</td>
                        <td>Returns the string encoding method as a string. In the case of Japanese environment, "Shift_JIS" is returned.</td>
                    </tr>
                    <tr>
                        <td>"charset"</td>
                        <td>Returns the character set numerically. For Japanese environment, 128 is returned.</td>
                    </tr>
                    <tr>
                        <td>"codepage"</td>
                        <td>Returns the code page numerically. For Japanese environment, 932 is returned.</td>
                    </tr>
                    <tr>
                        <td>"lang"</td>
                        <td>Returns the language identifier as a string. In the case of Japanese environment, "ja" is returned.</td>
                    </tr>
                    <tr>
                        <td>"country_code"</td>
                        <td>Returns the country code of the international call code as a number. In the case of Japanese environment, 81 is returned.</td>
                    </tr>
                    <tr>
                        <td>"mail_encoding"</td>
                        <td>Returns a string of the standard encoding methods used in email. In the case of Japanese environment, "ISO-2022-JP" is returned.</td>
                    </tr>
         </table>
    </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var cc = getLocaleInfo ("lang");
if (cc == "ja") {
    MessageBox (" Hello ");
} else {
    MessageBox ("Hello");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





