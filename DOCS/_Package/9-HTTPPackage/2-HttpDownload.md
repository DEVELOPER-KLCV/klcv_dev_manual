---
layout: default

parent: 9. HTTP Package
has_children: true

title: HttpDownload Class
nav_order: 2
permalink: /package/httppackage/httpdownload

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

Parallel download class. Execute it in a thread separate from the Biz / Browser GUI.

**Default properties and ValueType**

There are no default properties. The ValueType specification is invalid.

**About specifying the download server**
 
**When downloading from the same server as CRS**
```
HttpDownload down;
var down = new HttpDownload();
var down = new HttpDownload(getHttpSession());
```

**When specifying a server**
```
var down = new HttpDownload("http//PrintServer");
var session = findHttpSession("http://PrintServer");
var down = new HttpDownload(session); /* session must have a valid Protocol and Server set */ 
```
See the [AddURL](/package/httppackage/httpdownload/methods/addurl) method for how to specify the URL.