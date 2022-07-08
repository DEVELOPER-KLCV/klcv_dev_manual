---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.AfterUserSort Event
nav_order: 6
permalink: /package/extension5/sspread/events/afterusersort
---
# {{ page.title }}

Occurs after the data sort is complete.

Specifically, an event occurs during the following operations.

- User clicks column header

- Set $ColUserSortIndicatorAscending (sort / ascending order) and $ColUserSortIndicatorDescending (sort / descending order) in the <a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a> property.

- Set $UserColActionSort (sort / indicator display) and $UserColActionSortNoIndicator (sort / indicator hidden) in the <a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a>  property.

The following child objects are attached to the Event object.

| Type   |    Name   | Description                        |
|--------|:---------:|------------------------------------|
| Number | **_Col_** | Column number of the sorted column |

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
AllowRowMove = $TRUE;
Function OnAfterUserSort (e) {
    MessageBox ( str ( e.Col ) + " columns have been sorted ");
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a>, <a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a> property<br>
<a href="/package/extension5/sspread/events/beforeusersort">BeforeUserSort</a> event












