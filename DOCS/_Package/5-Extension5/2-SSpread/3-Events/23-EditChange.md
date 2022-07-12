---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.EditChange Event
nav_order: 23
permalink: /package/extension5/sspread/events/editchange
---
# {{ page.title }}

Occurs when the value is changed in a cell whose input mode is ON (edited state).

The following child objects are attached to the Event object.

| Type   |    Name   | Description                                       |
|--------|:---------:|---------------------------------------------------|
| Number | **_Col_** | Column number of the cell whose value has changed |
| Number | **_Row_** | Row number of the cell whose value has changed    |

This event is fired for every single character entered, but there is no guarantee that the OnEditChange event handler will be called immediately. In other words, it is not suitable for processing that checks errors for each character.

Also, it is not recommended to change the properties related to the entire spreadsheet or change the settings that cause inconsistencies in the cell being edited in the event handler that occurs while editing the cell, as it may not work properly.

Example of usage<br>
```
Function OnEditChange (e) {
    print (e.Col, e.Row, GetText (e.Col, e.Row), "\ n");
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/editenteraction">EditEnterAction</a>, <a href="/package/extension5/sspread/properties/editmode">EditMode</a>, <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a>, <a href="/package/extension5/sspread/properties/editmodereplace">EditModeReplace</a> property <br><a href="/package/extension5/sspread/events/editerror">EditError</a>, <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a>, <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a> event