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
| [GetMonth](/package/system/date/methods/getMonth) 	|Returns the month of the date in local time |
| [GetDate](/package/system/date/methods/getDate) 	|Returns the day part of a date in local time |
| [GetDay](/package/system/date/methods/getDay) 	|Returns the day of the week for a date in local time |
| [GetHours](/package/system/date/methods/getHours) 	| Returns the hour part of local time|
| [GetMinutes](/package/system/date/methods/getMinutes) 	| Returns the minutes part of local time|
| [GetSeconds](/package/system/date/methods/getSeconds) 	|Returns the seconds part of local time |
| [GetMilliSeconds](/package/system/date/methods/getMilliSeconds) 	| Returns the millisecond portion of local time |
| [GetUTCFullYear](/package/system/date/methods/getUTCFullYear) 	| Returns the year of the date in UTC |
| [GetUTCMonth](/package/system/date/methods/GetUTCMonth) 	| Returns the month of the date in UTC |
| [GetUTCDate](/package/system/date/methods/GetUTCDate) 	| Returns the day part of a date in UTC |
| [GetUTCDay](/package/system/date/methods/GetUTCDay) 	| Returns the day of the week for a UTC date |
| [GetUTCHours](/package/system/date/methods/GetUTCHours) 	| Returns the hours component of a date in UTC |
| [GetUTCMinutes](/package/system/date/methods/GetUTCMinutes) 	| Returns the minutes component of a date in UTC |
| [GetUTCSeconds](/package/system/date/methods/GetUTCSeconds) 	| Returns the seconds component of a date in UTC |
| [GetUTCMilliSeconds](/package/system/date/methods/GetUTCMilliSeconds) 	| Returns the milliseconds component of a date in UTC |
| [GetTimezoneOffset](/package/system/date/methods/GetTimezoneOffset) 	| Returns the time zone offset as a value in minutes |
| [SetTime](/package/system/date/methods/SetTime) 	| Set date and time directly |
| [SetFullYear](/package/system/date/methods/SetFullYear) 	| Set the year part in local time |
| [SetMonth](/package/system/date/methods/SetMonth) 	| Set the month part in local time |
| [SetDate](/package/system/date/methods/SetDate) 	| Set the date part in local time |
| [SetHours](/package/system/date/methods/SetHours) 	| Set the hours part in local time |
| [SetMinutes](/package/system/date/methods/SetMinutes) 	| Set the minutes part in local time |
| [SetSeconds](/package/system/date/methods/SetSeconds) 	| Set the seconds part in local time |
| [SetMilliSeconds](/package/system/date/methods/SetMilliSeconds) 	| Set the milliseconds part in local time |
| [SetUTCFullYear](/package/system/date/methods/SetUTCFullYear) 	| Set the year part in UTC |
| [SetUTCMonth](/package/system/date/methods/SetUTCMonth) 	| Set the month part in UTC |
| [SetUTCDate](/package/system/date/methods/SetUTCDate) 	| Set the day part in UTC |
| [SetUTCHours](/package/system/date/methods/SetUTCHours) 	| Set the hour part in UTC |
| [SetUTCMinutes](/package/system/date/methods/SetUTCMinutes) 	| Set the minutes part in UTC |
| [SetUTCSeconds](/package/system/date/methods/SetUTCSeconds) 	| Set the seconds part in UTC |
| [SetUTCMilliSeconds](/package/system/date/methods/SetUTCMilliSeconds) 	| Set the milliseconds part in UTC |
| [ToDateString](/package/system/date/methods/ToDateString) 	| Returns the date as a string |
| [ToInternetString](/package/system/date/methods/ToInternetString) 	| Returns the date as a string in RFC822 format<br>**<small>Added since Version 4.1.0</small>**<br>**<small>Not supported in Mobile</small>** |
| [ToLocaleDateString](/package/system/date/methods/ToLocaleDateString) 	| Returns the date as a string in locale format |
| [ToLocaleString](/package/system/date/methods/ToLocaleString) 	| Returns the date and time as a locale-formatted string |
| [ToLocaleTimeString](/package/system/date/methods/ToLocaleTimeString) 	| Returns the time as a string in locale format |
| [ToString](/package/system/date/methods/ToString) 	| Returns the date and time as a string |
| [ToTimeString](/package/system/date/methods/ToTimeString) 	| Returns the time as a string |
| [ToUTCString](/package/system/date/methods/ToUTCString) 	| Returns the date as a UTC string |
| [ValueOf](/package/system/date/methods/ValueOf) 	| Returns the time elapsed since UTC reference time, in milliseconds. |

Static Methods

|Name       | Description |
|----------	|-------------|
| [Parse](/package/system/date/methods/parse)  |Parses the date string |
| [UTC](/package/system/date/methods/utc) 	| Returns the interval between 0:00:00, January 1, 1970, UTC, and the specified date, in milliseconds. |