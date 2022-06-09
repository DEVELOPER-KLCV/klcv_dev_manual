---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetUserSip Property
nav_order: 32
permalink: /package/standard/root/methods/setusersip
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Perform mapping between the SIP ID that can be specified in the <a href="/package/standard/root/methods/showsip">ShowSIP</a> method or the <br><a href="/package/standard/editobject/properties/imemode">EditObject.IMEMode</a> property and the SIP control plug-in DLL.<br><small><span style="color:red">Can only be used with Mobile<br>Added since Mobile Ver.4.0.0</span></small><br><br>
    
    <b><i>SIP control plug-in DLL</i></b><br>

    Handy terminals for business use may be equipped with a model-specific SIP, and SIP control may be controlled by a unique SDK and API.<br><br>

    In the conventional Biz / Browser Mobile, there is no way to control the SIP unique to the terminal, and the input mode can be specified only for general Windows, so it was not possible to use SIP-specific functions.<br><br>

    By using the SIP control plug-in, it is possible to fully utilize the simplicity of SIP control of Biz / Browser and the SIP functions unique to the terminal.<br><br>

    If you set the SIP ID mapped by the SetUserSip method to the ShowSIP method or IMEMode property, each specified value will be redirected to the plug-in.<br><br>
    
    The plug-in performs its own SIP control by determining the specified value and calling the API provided by the SDK.<br><br>
    
    SIP ID should always be specified to redirect to the SIP control plug-in.<br><br>

    For example, when closing SIP via a plug-in, <br>

    IMEMode = $ SIP_CLOSE;<br>

    is invalid and it should be specified as below.<br>

    IMEMode = $ SIP_USER1 + $ SIP_CLOSE;
    
    </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetUserSip( <b>sipId</b>, <b>dll</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>sipId</b></td>
    <td>Specify the SIP ID to set the plug-in DLL. Specify one of the following values.<br>IDs of $ SIP_USER1 to 3 are provided for plug-in assignment, but it is also possible to specify an existing ID (such as $ SIP_HIRAKATA) and overwrite the existing SIP settings.<br>
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
.tg .tg-8zwo{font-style:italic;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7jy7">Constant</th>
    <th class="tg-7jy7">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ SIP_HIRAKATA</td>
    <td class="tg-f8tv">"Hiragana / Katakana" mode</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ SIP_ROMAJI</td>
    <td class="tg-f8tv">"Romaji / Kana" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWINPUT</td>
    <td class="tg-8zwo">"Handwriting input" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_HWSEARCH</td>
    <td class="tg-0lax">"Handwriting search" mode</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER1</td>
    <td class="tg-0lax">For SIP control plug-in assignment</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER2</td>
    <td class="tg-0lax">For SIP control plug-in assignment</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ SIP_USER3</td>
    <td class="tg-0lax">For SIP control plug-in assignment</td>
  </tr>
</tbody>
</table>

<br>IDs of $ SIP_USER1 to 3 are provided for plug-in assignment, but it is also possible to specify an existing ID (such as $ SIP_HIRAKATA) and overwrite the existing SIP settings.</td>
  </tr>
  <tr>
    <td>String <b>dll</b></td>
    <td>Specify the file name of the SIP control plug-in DLL.<br> The dll should be placed in the same dll folder as the plug-in used by the CallDll method.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetUserSip($SIP_USER1, "UserSip.dll");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/showsip">ShowSIP</a> method<br><a href="/package/standard/editobject/properties/imemode">EditObject.IMEMode</a> property</td>
  </tr>
</table>



