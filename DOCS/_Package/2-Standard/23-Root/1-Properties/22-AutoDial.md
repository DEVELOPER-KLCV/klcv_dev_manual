---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.AutoDial Property
nav_order: 22
permalink: /package/standard/root/properties/autodial
---
# {{ page.title }}
<br>

Specify the dial-up control method when dial-up is required when accessing the network.

 

Specify one of the following values

|        Constant        | Description                                                                                                                                                                                                                                                                   |
|:----------------------:|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Root.Off               | It does not dial up automatically. Also , the line will not be disconnected when Biz / Browser Mobile is closed.                                                                                                                                                              |
| Root.Up                | Dial-up will be performed automatically if necessary.                                                                                                                                                                                                                         |
| Root.Down              | The line will be disconnected when Biz / Browser is closed. However, if the line is controlled by another application, it may not be disconnected.                                                                                                                        |
| Root.DownAlt           | Only valid for Windows Mobile. The line will be disconnected when Biz / Browser is closed. The difference from Down is that it disconnects by emulating the "End Call" button. If specified on a Windows CE, it is considered the same as Down . <br><small><span style="color:red">Added since Mobile Ver.3.2.2</span><small> |
| Root.Up+Root.Down(Alt) | It is a combination of Root.Up and Root.Down (Alt)                                                                                                                                                                                                                            |

The following values can be added

|   Constant  | Description                                                                    |
|:-----------:|--------------------------------------------------------------------------------|
| Root.Silent | Only valid for Windows CE. Does not display a dialog when dialing up. <br><small><span style="color:red">Added since Mobile Ver.3.2.2</span><small>     |

The default value is Root.Up + Root.Down.

 

For Windows CE machines, it is affected by the Root.DialEntry property.

<br><small><span style="color:red">Can only be used with Mobile</span></small>
<br><small><span style="color:red">Only supported in Mobile Ver.3.0.1 and later version</span></small>
<br><small><span style="color:green">Supported in Windows CE since Mobile Ver.3.0.1 and later version</span></small>