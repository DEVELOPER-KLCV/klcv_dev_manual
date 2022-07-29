---
layout: default

grand_parent: NetObject Class
parent: Methods
has_children: false
title: NetObject.Get Method
nav_order: 3
permalink: /package/system/netobject/methods/get
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Download CRS file from the WEB server and execute it.<br><br>Search the target CRSfile specified in the URL in the following order.<ol><li>
    If it is already cached on the loacal computer, it will be read from the cache.</li><li>If it is included in the <a href="/bizBrowserV/3/3-5/t">CRSarchive</a> (CARfile) imported in advance, it will be read from archive.</li><li>Send a request to the web server and get the CRS file.</li></ol><br> The acquire content is immediately excuted as a CRS script. If possible, save the CRS file obtained from the WEB server in cache.<br>For cache control, see controlling cache with HTTPheaders below.<br><br>If you do not specify <b><i>param</i></b>, thebe sent HTTPGET.<br>If you specify <b><i>param</i></b>thebe sent HTTPPOST.<br><br>If the web server does not return 200 ($HTTP_OK) for the HTTP status code, a CRS-331 exeption will occur.<br><small><span style="color:red">Added since Ver.4.0.5., Mobile Ver.3.0.0 It is now possible to raise arbitrary excption using HTTP response headers. SEE <a href= "/package/system/netobject/methods/get#conversion-rule-for-each-type-of-object-specified-in-param">Controlling Exceptions with HTTP Headers</a> below for more informartion.</span></small><br><br>The current scope (this) of the acquired CRSscript is the object that excuted the Get method. For example, excuting the get method inside the OnTouch event handler of the Button class will create an object as a child of the Button object. When getting the CRS that defines the screen (Form claass), it is common to excute the Get method on the Root object. (//) or Form object.<br><br>The Get method does not return until the excution of the acquired CRS script is completed.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Get( <b>URL</b> [, <b>param1</b> [, <b>param2</b> [, ... ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL of the CRS file<br>The URL is determined by the following rules.<br><br><b><u>Specified from protocol</u></b><br>If specified from a protocol such as http:// , the request will be sent as it is.The URL cannot start with the host name. If want to specify the host name, be sure to specify it from the protocol.<br>example:-<br>Get("http://server/path/form1.crs");<br>Get("https://server/path/form1.crs");
    <br><br><b><u>Absolute path specification</u></b><br>URLs starting with "/" are absolute paths. Send the request to the server that downloaded the CRS file that executed the Get method.<br>Example:- When the CRS that executes the Get method is downloaded from http://server/path1/form1.crs<br>Get("/path2/form2.crs");<br>↓<br>Get("http://server/path2/form2.crs")
    <br><br><b><u>Relative path specification</u></b><br>URLs that do not start with "/" are relative paths. Send the request to the same path on the server where you downloaded the CRS file that executed the Get method.<br>Example:- When the CRS that executes the Get method is downloaded from http://server/path/form1.crs<br>Get("form3.crs");<br>↓<br>Get("http://server/path/form3.crs")<br><br>Using the APPROOT property of the <a href="/package/standard/root/sysobject">SYS object</a> behaves differently than above with relative path specifications. The APPROOT property is left for compatibility with versions prior to version 3.0 and should not be used in new programs.</td>
    </tr>
  <tr>
    <td>Object <b>param</b></td>
    <td>Parameters to be added to the request.<br>There is no limit to the number of parameters that can be specified.<br>It is converted to a character string and added to the request according to the<a href="/package/system/netobject/methods/get#conversion-rule-for-each-type-of-object-specified-in-param"> conversion rules for each object type</a> specified in the parameter.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CRS-331</td>
    <td>Communication error<br>The Exception object has the following structure.<br><code><pre>Exception {
    String RequestURL;  /* URL of the request that caused the exception */
    Number StatusCode;  /* HTTP status code */
    String ContentType; /* Content-Type of HTTP header */
    String Body;        /* Response body */
}</pre></code></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnTouch(e) {
    //.Form1.Delete();
    //.Get("Form2.crs");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/netobject/methods/cache">Cache</a>, <a  href="/package/csvpackage/csvdocument/methods/get">CSVDocument.Get</a> methods</td>
  </tr>
</table>

### Conversion rule for each type of object specified in param
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-xt05">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">String literal<br>例）"key=100"、"abc"</td>
    <td class="tg-0lax">When "=" is included in the specified character string, the left side of "=" is the parameter name and the right side is the data value.<br>If "=" is not included, "argN" ( N is a number according to the position of the parameter) is used as the parameter name, and the entire character string is used as the data value.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric literal<br>Example) 100 , 1.2</td>
    <td class="tg-0lax">"argN" ( N is a number according to the position of the parameter) is the parameter name, and the character string converted in the standard format of Number type is the data value.</td>
  </tr>
  <tr>
    <td class="tg-0lax">String<br>UString</td>
    <td class="tg-0lax">The object name is the parameter name, and the entire character string of the Value property is the data value. UString is converted to String .<br><small><span style="color:green">Since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change501.gif" width="50" height="12">,if more anonymous object is specified, it behaves the same as a string literal.</span></small></td>
  </tr>
  <tr>
    <td class="tg-0lax">Number<br>Fixed<br>Date</td>
    <td class="tg-0lax">The object name is the parameter name and the Value property is the data value.<br>The value of the Value property is converted to a string in the standard format according to the data type.<br><small><span style="color:green">Since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change501.gif" width="50" height="12">,if more anonymous object is specified, use "argN" ( N is a number according to the position of the parameter) in the parameter name.</span></small></td>
  </tr>
  <tr>
    <td class="tg-0lax">Spread<br>PulldownList<br>OptionButton<br>ListBox (single selection)</td>
    <td class="tg-0lax">It is a single-selection composite object.<br>The object name is the parameter name and the Value property is the data value.<br>The Value property represents the currently selected element. -1 if no element is selected .<br>The value of the Value property is converted to a string.</td>
  </tr>
  <tr>
    <td class="tg-0lax">CheckBox<br>ListBox (multiple selection)</td>
    <td class="tg-0lax">This is a multi-select compound object.<br>The object name is the parameter name, and the Selected property of each element ( CheckItem , ListItem ) is the data value.<br>Parameters are generated for all elements.<br>example)<br><code><pre>CheckBox CheckBox1 {<br>   CheckItem item[3];<br>}<br></pre></code>In this example, three parameters with the same name "CheckBox1" are generated, and the data values are item [0] .Selected , item [1] .Selected , and item [2] .Selected .<br>It is "1" in the selected state and "0" in the non-selected state .</td>
  </tr>
  <tr>
    <td class="tg-0lax">Root<br>Dialog<br>Doc<br>Form<br>Record<br>TabForm<br>SplitterFrame<br>SplitterForm<br>GraphAxis<br>SpreadRow</td>
    <td class="tg-0lax">Finds child objects and uses all found objects as parameters.<br>The object name is the parameter name and the default property is the data value.<br>example)<br><code><pre>Form Form1 {<br>   Button Button1;<br>   Label Label1;<br>   String String1;<br>}<br></pre></code>In this example, we will generate three parameters named "Button1" , "Label1" , and "String1" , and set their default properties as data values.<br>The value of the default property is converted to a string in the standard format according to the data type.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Objects other than above</td>
    <td class="tg-0lax">The object name is the parameter name and the default property is the data value.<br>The value of the default property is converted to a string in the standard format according to the data type.<br><small><span style="color:green">Since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change501.gif" width="50" height="12">,if more anonymous object is specified, use "argN" ( N is a number according to the position of the parameter) in the parameter name.</span></small></td>
  </tr>
</tbody>
</table>

### Controlling the cache with HTTP headers
If the HTTP response header returned from the server is specified as no-cache by the standard HTTP headers Cache-Control header and Pragma header, Biz / Browser will not cache the retrieved file.
<br><br><small><span style="color:red">Featurs added since Ver.4.0.6, Mobile Ver.3.0.0--></span></small><br>
The CRS-Cache-Control header, which is a Biz / Browser - specific header, can control the cache in preference to the standard HTTP header cache control ( Cache-Control , Pragma header).
```
CRS-Cache-Control: no-cache
or
CRS-Cache-Control: cache
 ```
If no-cache is specified in the CRS-Cache-Control header, it will not be cached. If cache is specified, it will be cached.

This function can be used when you want to perform different cache control in Biz / Browser with a proxy server that relays HTTP messages . For example, if you specify no-cache in the Cache -Control header and cache in the CRS-Cache-Control header, it will not be cached by the relay proxy server, and Biz / Browser can instruct the cache operation.
<br><small><span style="color:red"><-- Up to here</span></small>

### Controlling exceptions with HTTP headers
<br><small><span style="color:red">Featurs added since Ver.4.0.5, Mobile Ver.3.0.0--></span></small><br>
Arbitrary exceptions can be raised by using the header of the HTTP response returned from the server . This function can be used for application-specific communication error handling.
By specifying the CRS-Exception header in the response header with HTTP status code 200 ( $ HTTP_OK ), you can raise an exception even in normal communication.

Specify the CRS-Exception header in the following format.

CRS-Exception: Method: <b>Method</b> ; Code: <b>Code</b> ; Message: <b>Message</b> ;

Method , Code , and Message correspond to properties of the same name in the <a href="/package/system/exception/">Exception</a> class.
The content of the Method is set in the <a href="/package/system/exception/properties/method">Method</a> property. If Method is not specified, "Server-Error" will be displayed.
The contents of the Code are set in the <a href="/package/system/exception/properties/code">Code</a> property. If Code is not specified, it will be 0 .
The content of the Message is set in the <a href="/package/system/exception/properties/message">Message</a> property. If you do not specify Message , the entire CRS-Exception header is set to Message .

The Exception object of the exception that occurs has the same structure as the CRS-331 exception and stores the same information ( RequestURL , StatusCode , etc.).
<br><small><span style="color:red"><-- Up to here</span></small>

