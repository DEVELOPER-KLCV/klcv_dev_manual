---
layout: default
has_children: true

title: 2. Biz / Browser Overview
nav_order: 2
permalink: /bizBrowserV/2-Overview/
---

# {{ page.title }}


{: .no_toc }

Biz / Browser is executed by an interpreter with a built-in script written in a scripting language similar to JavaScript called CRS. Biz / Browser adopts HTTP as the basic input / output method, and can operate by downloading CRS (including script code, data, screen definition, etc.) from the WEB server.

Biz / Browser is mainly used for routine business applications. It cannot handle multimedia data (video, sound, etc.), but it has a function to handle text information efficiently, a form printing function considering page control, cooperation with PrintStream, which is a form tool of another product, and between items. It has a full range of functions required by applications that perform routine tasks, such as focus movement control, calculation between items, and calculation functions using built-in functions.

Since Biz / Browser is mainly used on the network, it is equipped with a powerful cache system controlled by the application to reduce the amount of data passing through the line. The CRS script downloaded from the WEB server is saved in the cache in a compiled binary format. Therefore, communication other than dynamic fluctuation data does not occur for the screen once displayed. With this structure, even if a client-server connection is made with a low-speed line of about 64k, it can operate at a sufficiently practical speed. With the conventional method, it is possible to build a routine business application that supports a wide area network, which was difficult for a practical system.

---

### Biz / Browser usage system overall conceptual diagram

<br>

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/intro/intro.files/image001.jpg" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>
