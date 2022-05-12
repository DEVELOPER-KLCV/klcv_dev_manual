---
layout: default

grand_parent: 1. System Package
parent: Date Class

title: Methods
nav_order: 2
permalink: /package/system/date/methods

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following methods are defined in the Date class.

|Name       | Description |
|----------	|-------------|
| [Constructor](/package/system/date/methods/constructor)  |Initialize the Date object |
| [GetTime](/package/system/date/methods/gettime) 	| Returns the stored time |
| [GetFullYear](/package/system/date/methods/getfullyear) 	| Returns the year of the date in local time |
| [GetMonth](/package/system/date/methods/getmonth) 	|Returns the month of the date in local time |
| [GetDate](/package/system/date/methods/getdate) 	|Returns the day part of a date in local time |
| [GetDay](/package/system/date/methods/getday) 	|Returns the day of the week for a date in local time |
| [GetHours](/package/system/date/methods/gethours) 	| Returns the hour part of local time|
| [GetMinutes](/package/system/date/methods/getminutes) 	| Returns the minutes part of local time|
| [GetSeconds](/package/system/date/methods/getseconds) 	|Returns the seconds part of local time |
| [GetMilliSeconds](/package/system/date/methods/getmilliseconds) 	| Returns the millisecond portion of local time |
| [GetUTCFullYear](/package/system/date/methods/getutcfullyear) 	| Returns the year of the date in UTC |
| [GetUTCMonth](/package/system/date/methods/getutcmonth) 	| Returns the month of the date in UTC |
| [GetUTCDate](/package/system/date/methods/getutcdate) 	| Returns the day part of a date in UTC |
| [GetUTCDay](/package/system/date/methods/getutcday) 	| Returns the day of the week for a UTC date |
| [GetUTCHours](/package/system/date/methods/getutchours) 	| Returns the hours component of a date in UTC |
| [GetUTCMinutes](/package/system/date/methods/getutcminutes) 	| Returns the minutes component of a date in UTC |
| [GetUTCSeconds](/package/system/date/methods/getutcseconds) 	| Returns the seconds component of a date in UTC |
| [GetUTCMilliSeconds](/package/system/date/methods/getutcmilliseconds) 	| Returns the milliseconds component of a date in UTC |
| [GetTimezoneOffset](/package/system/date/methods/gettimezoneoffset) 	| Returns the time zone offset as a value in minutes |
| [SetTime](/package/system/date/methods/settime) 	| Set date and time directly |
| [SetFullYear](/package/system/date/methods/setfullyear) 	| Set the year part in local time |
| [SetMonth](/package/system/date/methods/setmonth) 	| Set the month part in local time |
| [SetDate](/package/system/date/methods/setdate) 	| Set the date part in local time |
| [SetHours](/package/system/date/methods/sethours) 	| Set the hours part in local time |
| [SetMinutes](/package/system/date/methods/setminutes) 	| Set the minutes part in local time |
| [SetSeconds](/package/system/date/methods/setseconds) 	| Set the seconds part in local time |
| [SetMilliSeconds](/package/system/date/methods/setmilliseconds) 	| Set the milliseconds part in local time |
| [SetUTCFullYear](/package/system/date/methods/setutcfullyear) 	| Set the year part in UTC |
| [SetUTCMonth](/package/system/date/methods/setutcmonth) 	| Set the month part in UTC |
| [SetUTCDate](/package/system/date/methods/setutcdate) 	| Set the day part in UTC |
| [SetUTCHours](/package/system/date/methods/setutchours) 	| Set the hour part in UTC |
| [SetUTCMinutes](/package/system/date/methods/setutcminutes) 	| Set the minutes part in UTC |
| [SetUTCSeconds](/package/system/date/methods/setutcseconds) 	| Set the seconds part in UTC |
| [SetUTCMilliSeconds](/package/system/date/methods/setutcmilliseconds) 	| Set the milliseconds part in UTC |
| [ToDateString](/package/system/date/methods/todatestring) 	| Returns the date as a string |
| [ToInternetString](/package/system/date/methods/tointernetstring) 	| Returns the date as a string in RFC822 format<br>**<small>Added since Version 4.1.0</small>**<br>**<small>Not supported in Mobile</small>** |
| [ToLocaleDateString](/package/system/date/methods/tolocaledatestring) 	| Returns the date as a string in locale format |
| [ToLocaleString](/package/system/date/methods/tolocalestring) 	| Returns the date and time as a locale-formatted string |
| [ToLocaleTimeString](/package/system/date/methods/tolocaletimestring) 	| Returns the time as a string in locale format |
| [ToString](/package/system/date/methods/tostring) 	| Returns the date and time as a string |
| [ToTimeString](/package/system/date/methods/totimestring) 	| Returns the time as a string |
| [ToUTCString](/package/system/date/methods/toutcstring) 	| Returns the date as a UTC string |
| [ValueOf](/package/system/date/methods/valueof) 	| Returns the time elapsed since UTC reference time, in milliseconds. |

Static Methods

|Name       | Description |
|----------	|-------------|
| [Parse](/package/system/date/methods/parse)  |Parses the date string |
| [UTC](/package/system/date/methods/utc) 	| Returns the interval between 0:00:00, January 1, 1970, UTC, and the specified date, in milliseconds. |