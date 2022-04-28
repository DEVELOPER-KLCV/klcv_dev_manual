---
layout: default

grand_parent: Byte Array Class
parent: Methods
has_children: false
title: ByteArray constructor
nav_order: 1
permalink: /package/system/bytearray/methods/constructor
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the ByteArray object.<br><br>If no argument is specified, it will be initialized empty.<br>Multiple values can be specified for the argument, and the specified values are combined and initialized.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var barr = new ByteArray ([<b>data_1 [, data_2 , [, ... [, data_n ]]]]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">ByteArray object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>data_n</i></b></td>
    <td>Specify the data to be set as the default value.<br>You can specify strings, ByteArray objects, and binary data. Otherwise, it will be converted to a string.<small>The following specifications have been added to Mobile, Ver.5.0.0, AI Ver.1.0.1</small><br><br>If a positive integer is passed as an argument, it will be stored as binary data as it is. This makes it possible to create non-character data strings such as control codes.<br>Numerical values are stored in little endian as 1 byte from 0 to 255, 2 bytes from 256 to 65535, and 4 bytes from 65536 to 4294967295 (hexadecimal FFFFFFFF).<br>Numerical values outside the above range and numerical values including decimal numbers are stored as character strings.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var b1 = new ByteArray(file.Read());
var b2 = new ByteArray("sample", "test");
var b3 = new ByteArray(response.Read());</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



