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
    <td colspan="2">Set your own menu in the menu bar of Biz / Browser.<br><br> Use XML to define the menu. The hierarchical structure of XML becomes the hierarchical structure of the menu as it is. The <a href="/package/standard/root/events/menuselected">MenuSelected</a> event is fired when a menu is selected.<br><br> If Biz / Browser is running inside Internet Explorer, this method is invalid because the menu is not displayed.<br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
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
    <td><a href="/package/xmlpackage/xmldocument">XmlDocument</a>
 object that represents the contents of the menu <br> XmlDocument whose<a href="/package/xmlpackage/xmldomimplementation/methods/constructor#about-xml-with-a-unicode-internal-character-code">character code is  Unicode</a> cannot be specified.<br><br><small><span style="color:green">The following specifications have been added since Ver.5.0.1</span></small><br>If the argument is omitted or null is passed to the argument, the menu is returned to the standard.</td>
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


<b><i>Menu definition XML format</i></b>

Menu element

| Element Name | Description                                                                                | Parent Element | Attributes                 |
|--------------|--------------------------------------------------------------------------------------------|----------------|----------------------------|
| menu         | Top-level menu element. Specify the items displayed in the menu bar.                       | root           | title、checked、grayed     |
| menuitem     | It is a menu element. It becomes the parent item of each item of the menu and the submenu. | menu、menuitem | id、title、checked、grayed |
| separator    | It is a separator element. Insert a separator line in the menu.                            | menu、menuitem | none                       |


Menu attributes

| Attributes Name | Description                                                                                                           | Specifiable value        |
|-----------------|-----------------------------------------------------------------------------------------------------------------------|--------------------------|
| id              | The menu ID . The ID of the selected menu is set in the <a href="/package/standard/root/events/menuselected">MenuSelected</a> event.                                           | Integer value (0～65535) |
| title           | The title displayed in the menu.                                                                                      | String                   |
| checked         | Whether or not there is a check mark. If set to "true" , a check mark will be displayed on the left side of the menu. | "true"                   |
| grayed          | Specify whether to enable / disable the menu. Setting "true" disables the menu.                                       | "true"                   |





