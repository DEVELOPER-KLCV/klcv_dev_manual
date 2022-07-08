---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.Advance Event
nav_order: 1
permalink: /package/extension5/sspread/events/advance
---
# {{ page.title }}

Occurs when trying to move focus out of the spreadsheet area with the Tab or Direction keys.

Specifically, an event occurs during the following operations.

- Press the Tab key in the last cell<br>
- Press Shift + Tab in the first cell<br>
- Press the bottom of the direction key on the last line<br>
- Press the top of the direction key on the first line<br>

The following child objects are attached to the Event object.

| Type   | Name              | Description                                                              |
|--------|-------------------|--------------------------------------------------------------------------|
| Number | **_AdvanceNext_** | $TRUE under the Tab or Arrow keys $FALSE above Shift + Tab or arrow keys |

Operations with the Tab key will only fire if the <a href="/package/extension5/sspread/properties/processtab">ProcessTab</a> property is $TRUE.

Example of usage

```
ProcessTab = $TRUE;
Function OnAdvance(e) {
    if (e.AdvanceNext == $TRUE) {
        MoveFocus($NEXTFOCUS);
    } else {
        MoveFocus($PREVFOCUS);
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/processtab">ProcessTab</a> property



 
