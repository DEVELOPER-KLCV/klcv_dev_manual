---
layout: default

grand_parent: DisplayObject Class
parent: Methods
has_children: false
title: DisplayObject.PopupMenu Method
nav_order: 2
permalink: /package/standard/displayobject/methods/popupmenu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Display a pop-up menu.<br><small><p style="color:green">From Ver.5.0.0, it is possible to specify the menu by XML structure.<br>This removes the hierarchy restrictions and allows you to assign any ID.</p></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var id = obj.PopupMenu( <b>menu1</b> [, <b>menu2</b> [, <b>menu3</b> … ] ] )<br>or<br>var id = obj.PopupMenu( <b>menudef</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The ID number automatically assigned to the menu choices is returned.<br><br>The first element of the menu is 1 for the ID . In the hierarchical menu, "value of upper element *100 + n " is the ID number of the submenu.<br>If no menu is selected, 0 is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>menu</b></td>
    <td>Specify the menu choices as a character string.<br>If "-" is specified, the separator will be displayed.<br>A check mark is displayed by adding "*" to the first character .<br>If "~" is added to the first character, it will be invalid and cannot be selected.<br>If you specify an object that has child objects at the bottom, a hierarchical submenu is displayed. You can specify up to 4 levels of submenus.<br>If you specify an array, the array elements are expanded as menu items.</td>
  </tr>
  <tr>
    <td>XmlDocument <b>menudef</b></td>
    <td>Specifies the <a href="/package/xmlpackage/xmldocument">XmlDocument</a>object in the menu definition.<br>XmlDocument whose  <a href="/package/xmlpackage/xmldomimplementation/methods/constructor">XmlDOMImplementation.Unicode cannot be specified.<br><small><p style="color:red">Added since Ver.5.0.0</p><p style="color:blue">Not supported in Mobile, AI</p></small></a></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td rowspan="2">Example of use</td>
    <td><b>Example 1) Specification by character string</b></td>
    <td><code><pre>
var m1 = new String("menu1");  /*id=1*/
var m2 = new String("menu2");  /*id=2*/
var m3 = new String("-");
var m4 = new String("menu3");  /*id=4*/

var s1 = new String("*sub-menu1");  /* id=201 */
var s2 = new String("sub-menu2");   /* id=202 */
var s3 = new String("~sub-menu3");  /* id=203 */
m2.Append(s1);
m2.Append(s2);
m2.Append(s3);

var id = PopupMenu(m1, m2, m3, m4);
    </pre></code></td>
 </tr>
 <tr>
    <td><b>Example 2) XML specification</b></td>
    <td><code><pre>var x = new XmlDocument ();
x << xml <<-  
< ? xml version = "1.0" encoding = "SHIFT_JIS"? >
< menudefine>
    < menuitem id = "1" title = "menu1" />
    < menuitem id = "2" title = "menu2" checked = "true" />
    <separator />
    < menuitem id = "3" title = "menu3">
        < menuitem id = "11" title = "menu11" />
        < menuitem id = "12" title = "menu12" grayed = "true" />
        <separator />
        < menuitem id = "13" title = "menu13" checked = "true">
            < menuitem id = "21" title = "menu21" />
            < menuitem id = "22" title = "menu22" />
        </ menuitem>
    </ menuitem>
</ menudefine> 
->>;
var id = PopupMenu (x);
</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/object/methods/append">Append</a> method<br><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class</td>
  </tr></table>
