---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.CacheMode Property
nav_order: 4
permalink: /package/standard/root/properties/cachemode
---
# {{ page.title }}
<br>

Select the communication method to be cached.

 

Specify a combination of the following constants.

|         Constant        | Description                                                 |
|:-----------------------:|-------------------------------------------------------------|
| Root.CacheOff = 0       | Do not allow caching                                        |
| Root.CacheNetwork = 1   | Allows caching when communicating with http, https protocol |
| Root.CacheLocalFile = 2 | Allows caching when communicating with the file protocol    |

If the "Use local cache" option is not enabled on the setting screen displayed by selecting "View"-> "Settings" from the Biz / Browser menu, caching will not be performed regardless of the value of this property. 
 

The initial value is Root.CacheNetwork.

<br><small><span style="color:red">Added since Ver.5.0.2, AI Ver.1.0.2</span></small>
<br><small><span style="color:blue">Not supported in Mobile</span></small>