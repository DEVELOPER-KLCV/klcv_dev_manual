---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.ExternalCall Event
nav_order: 6
permalink: /package/standard/root/events/externalcall
---
# {{ page.title }}
<br>

Similar to the EventListener class, but easier to use than the EventListener class.<br>

It is possible to raise an event in Biz / Browser Mobile by sending a Windows API SendMessage or PostMessage to the top frame window of Biz / Browser Mobile.<br><br>

This makes it possible to generate an event from an external program or plug-in DLL, wait for a state change without polling, or make a pseudo-push type operation.<br><br>

The following child objects are attached to the Event object.

| Type   | Name        | Description                                              |
|--------|-------------|----------------------------------------------------------|
| Number | **_type_**  | Currently fixed to 0                                     |
| Number | **_param_** | LPARAM value specified in SendMessage or PostMessage API |


<b><u>Sender C program sample</u></b><br>

```
void SendEvent (LPARAM param)
{
    / * Get window message ID ( this ID is defined when Biz / Browser Mobile starts ) * /
    UINT WM_BBEXTERNALCALL = RegisterWindowMessage (_T ("BizBrowserExternalCall"));
 
    / * Get Biz / Browser Mobile top frame window * /
    HWND hWnd = FindWindow (_T ("Afx: BizBrowserMobileClass"), NULL);
 
    / * Send message * /
    PostMessage (WM_BBEXTERNALCALL, 0, param);
}
```


<br><small><span style="color:red">Can only be used in Mobile</span></small>
<br><small><span style="color:red">Supported since Mobile Ver.3.2.0 and later version.</span></small>