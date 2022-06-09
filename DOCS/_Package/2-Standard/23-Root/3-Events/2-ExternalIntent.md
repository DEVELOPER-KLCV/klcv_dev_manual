---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.ExternalIntent Event
nav_order: 2
permalink: /package/standard/root/events/externalintent
---
# {{ page.title }}
<br>
This event occurs when Biz / Browser AI receives an intent that meets the following conditions.

・ action = "jp.co.axissoft.biz.external.EXTERNAL_INTENT"

・ data = No provision (If specified, please note that other apps may be displayed as receivable depending on the value and the environment of the terminal)

・ category = "android.intent.category.DEFAULT"

If this intent is received while Biz / Browser is not running, Biz / Browser will not be started, CRS will be executed, or loaded.

Also, this event does not occur except for a security level of 0 (lowest).

The following child objects are attached to the Event object.

| Type   | Name      | Description                                                                                                                                                                             |
|--------|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Intent | extIntent | The received intent. See <a href="/package/extobjectpackage/intent">Intent</a> class for details. Use the <a href="/package/extobjectpackage/intent/methods/putextra">Intent.putExtra</a> method in the intent source app When data is stored, it can be obtained by using the <a href="/package/extobjectpackage/intent/methods/getextra">Intent.getExtra</a> method. |

<br><small><span style="color:red">Can only be used in AI</span></small><br><small><span style="color:red">Added since AI Ver.1.0.2</span></small>