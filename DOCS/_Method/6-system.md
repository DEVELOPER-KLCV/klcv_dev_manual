---
layout: default
has_children: true

title: System Functions
nav_order: 12
permalink: /method/system
has_toc: false
---

# {{ page.title }}

System functions are used to get information about the system.

| Name        	| Explanation                                                           	|
|-------------	|-----------------------------------------------------------------------	|
| [cachedate](/method/system/cachedate)             | Returns the latest update date of the cached information obtained from the currently connected serve<br>**<small>Added since Mobile Version 2.0.0</small>**|
| [changeProfile](/method/system/changeProfile)             | Change the operating environment of Biz / Browser<br>**<small>Not compatible with Mobile, AI</small>** |
| [debugMessage](/method/system/debugMessage)             | Display debug messages in Biz / Designer |
| [deleteCache](/method/system/deleteCache)               | Delete cache|
| [decodeURI](/method/system/decodeURI)           | URL decode the string |
| [encodeURI](/method/system/encodeURI)         | URL encode the string<br>**<small>Added since Mobile Version 2.0.0</small>** |
| [findHttpSession](/method/system/findHttpSession) | Finds and creates the specified HTTP session |
| [getBookmark](/method/system/getBookmark)     | Get bookmark list<br>**<small>Now behaves the same as the <a>Root.GetBookmark</a> method</small>** |
| [getHttpSession](/method/system/getHttpSession)       | Gets the current HTTP session |
| [getLocaleInfo](/method/system/getLocaleInfo)           | Get locale information<br>**<small>Added since Version 4.1.0</small>**<br>**<small>Not compatible with Mobile, AI</small>** |
| [getPrinterList](/method/system/getPrinterList)             | Get a list of printers<br>**<small>Not compatible with Mobile, AI</small>** |
| [hasConnectionLicense](/method/system/hasConnectionLicense)             | Check the connection license<br>**<small>Added since Version 4.1.0, Mobile Version 2.0.0</small>** |
| [importConnectionLicense](/method/system/importConnectionLicense)             | Import the connection license certificate<br>**<small>Added since Version 4.1.0, Mobile Version 2.0.0</small>** |
| [link](/method/system/link)             |  Executes a hyperlink<br>**<small>Now behaves the same as the <a>Runtime.ShellLink</a> method</small>|
| [print](/method/system/print)             | Display debug messages in Biz / Designer |
| [remBookmark](/method/system/remBookmark)             | Delete bookmark entry<br>**<small>Now behaves the same as the <a>Root.RemBookmark</a> method</small> |
| [setBookmark](/method/system/setBookmark)             | Add or change bookmark entries<br>**<small>Now behaves the same as the <a>Root.SetBookmark</a> method</small> |
| [setDefaultPrinter](/method/system/setDefaultPrinter)             | Set the default printer<br>**<small>Cannot be used with</small> |
| [setPalette](/method/system/setPalette)             | Change the color of the color constant |
| [syncObject](/method/system/syncObject)             | Forces GUI changes to take effect<br>**<small>Added since Version 5.0.0</small><br>**<small>Not compatible in Mobile</small> |
| [sysdate](/method/system/sysdate)             | Returns the current system date and time |