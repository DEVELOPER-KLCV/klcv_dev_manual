---
layout: default

grand_parent: 2. Standard Package
parent: Root Class

title: SYS Object
nav_order: 4
permalink: /package/standard/root/sysobject

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}
<br>

Biz / Browser builds a SYS object under the Root object at startup. It is generated before the application's CRS is loaded, so it can always be referenced in "//.SYS".

The SYS object is read-only. You cannot change the value, delete it with the <a href="/package/system/object/methods/delete">Delete</a> method, or add a subordinate object with the <a href="/package/system/object/methods/append">Append</a>
 method.


The properties of the SYS object are described below.



<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Name</th>
    <th class="tg-cqgq">Type</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">OS</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">A string that identifies the client OS<br><small><span style="color:green">Functions have been expanded since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change500.gif" alt="Image" width="50" height="12"> to support 64bit OS</span></small></td>
  </tr>
  <tr>
    <td class="tg-0pky">OS_VERSION</td>
    <td class="tg-c3ow">Number</td>
    <td class="tg-0pky">Client OS version number</td>
  </tr>
  <tr>
    <td class="tg-0pky">CLIENT</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Client browser name</td>
  </tr>
  <tr>
    <td class="tg-0pky">CLIENT_VERSION</td>
    <td class="tg-c3ow">Number</td>
    <td class="tg-0pky">Client browser version number</td>
  </tr>
  <tr>
    <td class="tg-0pky">PROXY</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Proxy server host name</td>
  </tr>
  <tr>
    <td class="tg-0pky">PROXY_PORT</td>
    <td class="tg-c3ow">Number</td>
    <td class="tg-0pky">Proxy server connection port number</td>
  </tr>
  <tr>
    <td class="tg-0pky">SERVER</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Server host name</td>
  </tr>
  <tr>
    <td class="tg-0pky">SERVER_PORT</td>
    <td class="tg-c3ow">Number</td>
    <td class="tg-0pky">Server connection port number</td>
  </tr>
  <tr>
    <td class="tg-0pky">USERNAME</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">(Always blank. It is left for compatibility with the past. The Windows login user name can be obtained with the <a href="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/rtm/rtm1m8.htm">Runtime.GetUserName</a> method.)</td>
  </tr>
  <tr>
    <td class="tg-0pky">APPROOT</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">(Remained for compatibility with the past)</td>
  </tr>
  <tr>
    <td class="tg-0pky">HOSTNAME</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Client computer name</td>
  </tr>
  <tr>
    <td class="tg-0pky">MODELNAME<br> </td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Manufacturer name, model name, etc. (manufacturer setting value)<br><small><span style="color:red">Supported by <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add320.gif" alt="Image" width="86" height="12"> and later version, and <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add.gif" alt="Image" width="18" height="12"></span></small></td>
  </tr>
  <tr>
    <td class="tg-0pky">PLATFORM</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Platform type<br><small><span style="color:red">Supported by <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add320.gif" alt="Image" width="86" height="12"> and later version, and <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add.gif" alt="Image" width="18" height="12"></span></small></td>
  </tr>
  <tr>
    <td class="tg-0pky">DEVICEID</td>
    <td class="tg-c3ow">String</td>
    <td class="tg-0pky">Device unique ID<br>In the Mobile version, the value is not guaranteed for Windows CE 5.0 or earlier models ( excluding Windows Mobile ).<br>A valid value is set only if the WindowsAPI KernelIoControl IOCTL_HAL_GET_UUID option is supported.<br>In the Android version, you can get the serial number set on the device.<br><small><span style="color:red">Supported by <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add321.gif" alt="Image" width="86" height="12"> and later version, and <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add.gif" alt="Image" width="18" height="12"></span></small></td>
  </tr>
  <tr>
    <td class="tg-0pky">LANGUAGEID</td>
    <td class="tg-c3ow">Number</td>
    <td class="tg-0pky">You can get the language ID ( locale ID / LCID) of the running OS .<br>Using this value makes it possible to determine the operating language in the CRS and branch the process.<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add450.gif" width="86" height="12"></span></small></td>
  </tr>
</tbody>
</table>

<br>
Usage Example

```
var message = strf("OSは %1 です", //.SYS.OS);
var title = strf("%1 Ver.%2", //.SYS.CLIENT, //.SYS.CLIENT_VERSION);
MessageBox(message, title);
```

<br><small><span style="color:green">The SYS object is no longer deleted when the DeleteChild method is executed on the Root object from Ver.5.0.0, Mobile Ver.4.5.0.</span></small>

<br>
**APPROOT Property**


<span style="color:red">The APPROOT property is left for compatibility with past Biz / Browser . Avoid using this property as much as possible.</span>

 
Get and set the position to be treated as "/" in the resource on the server. The value of this property can be changed exceptionally.

For example, if "/ APP1" is set and Get ("Proc1") with a relative path, the request will be sent at the URL http: // server-name / APP1 / Proc1. Also, if you use Get ("/ Proc1") with an absolute path, the request will be sent at the URL of http: // server-name / Proc1.

Starting with version 3.0, the APPROOT property must be downloaded by the same protocol, server, and port as the primary session (protocol, server, port when logged in) and the APPROOT property is specified. Use to determine the URL. Other than that, the URL is determined based on the specifications of the <a href="/package/system/netobject/methods/get">Get</a> method.

Note that the URL in the CAR file is also affected by the APPROOT property, so setting the APPROOT property will almost always prevent the CAR file from loading as intended. Therefore, <u>APPROOT cannot be specified and CAR files cannot be used at the same time.</u>





