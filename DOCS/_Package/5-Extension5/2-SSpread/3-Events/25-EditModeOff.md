---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.EditModeOff Event
nav_order: 25
permalink: /package/extension5/sspread/events/editmodeoff
---
# {{ page.title }}

Occurs when the cell input mode is turned off.

The following child objects are attached to the Event object.

| Type   | Name             | Description                                  |
|--------|:------------------:|----------------------------------------------|
| Number |     **_Col_**    | Active cell column number                    |
| Number |     **_Row_**    | Active cell row number                       |
| Number | **_ChangeMade_** | $TRUE if the value changes, $FALSE otherwise |

Example of usage<br>
```
String oldvalue;
Function OnEditModeOn (e) {
    oldvalue = GetText (e.Col, e.Row);
}
Function OnEditModeOff (e) {
    if (e.ChangeMade == $ TRUE) {
        if (GetText (e.Col, e.Row) == "") {
            MessageBox (" Enter ");
            SetText (e.Col, e.Row, oldvalue);
            EditMode = $ TRUE;
            return;
        }
    }
}
```

Related Item <br>
<a href="/package/extension5/sspread/properties/editenteraction">EditEnterAction</a>, <a href="/package/extension5/sspread/properties/editmode">EditMode</a>, <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a>, <a href="/package/extension5/sspread/properties/editmodereplace">EditModeReplace</a> property <br><a href="/package/extension5/sspread/events/editchange">EditChange</a>, <a href="/package/extension5/sspread/events/editerror">EditError</a>, <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a> event