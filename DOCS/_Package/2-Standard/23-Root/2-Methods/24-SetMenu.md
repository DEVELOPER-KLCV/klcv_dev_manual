---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetMenu Property
nav_order: 24
permalink: /package/standard/root/methods/setmenu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetMenu( [ <b>menuXML</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XMLDocument <b>menuXML</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var x = new XmlDocument();
    x << xml <<-
        &lt;?xml version="1.0" encoding="SHIFT_JIS"?&gt;
        &lt;menudefine&gt;
            &lt;menu title="File"&gt;
                &lt;menuitem id="11" title="Top" /&gt;
                &lt;separator /&gt;
                &lt;menuitem id="18" title="Setting" /&gt;
                &lt;menuitem id="19" title="End" /&gt;
            &lt;/menu&gt;
            &lt;menu title="Business"&gt;
                &lt;menuitem id="31" title="Daily report entry" /&gt;
                &lt;menuitem id="32" title="Attendance input" /&gt;
                &lt;menuitem id="33" title="Sales management" /&gt;
            &lt;/menu&gt;
            &lt;menu title="Master Admin"&gt;
                &lt;menuitem id="91" title="User information"&gt;
                &lt;/menuitem&gt;
            &lt;/menu&gt;
        &lt;/menudefine&gt;
    ->>;
    //.SetMenu(x);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/events/menuselected">MenuSelected</a> event<br><a href="/package/xmlpackage/xmldocument/">XmlDocument</a> class</td>
  </tr>
</table>


<b>Menu definition XML format</b>




