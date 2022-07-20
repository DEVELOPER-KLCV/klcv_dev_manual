---
layout: default

parent: 7. XML Package
has_children: true

title: XmlCharacterData Class
nav_order: 3
permalink: /package/xmlpackage/xmlcharacterdata

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

<a href="/img/Package/XML-XmlCharacterDataClass.png" target="_blank">
<img src="/img/Package/XML-XmlCharacterDataClass.png" alt="login image"></a>

The base class of the node that stores the string. It has the basic functionality of a node that stores strings.

The XmlCharacterData class is a virtual class and cannot instantiate itself.

The XmlCharacterData class is derived from the XmlNode class, and the properties and methods of the XmlNode class are also available. Similarly, a class derived from the XmlCharacterData class inherits the properties and methods defined in the XmlCharacterData class and the properties and methods defined in the XmlNode class and can be used in the same way.

For classes derived from XmlCharacterData, there is:<br>
[XmlText](/package/xmlpackage/xmltext)<br>
[XmlComment](/package/xmlpackage/xmlcomment)<br>
[XmlCDATASection](/package/xmlpackage/xmlcdatasection).