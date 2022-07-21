---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.EditMode Property
nav_order: 47
permalink: /package/extension5/sspread/properties/editmode
---
# {{ page.title }}

Set the input mode (edit mode of the text in the active cell).

Specify $TRUE to turn the input mode on and $FALSE to turn it off. The initial value is $FALSE.

***Turn on the input mode*** <br>
・ Key input on the cell<br>
・ Double-click the cell<br>
・ Set $TRUE for the EditMode property

***Turn off the input mode*** <br>
・ Press the Enter key<br>
・ Another cell becomes active<br>
・ Lose focus<br>
・ Set $FALSE in the EditMode property

The <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a>  event is fired when the input mode is ON, and the <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a>  event is fired when the input mode is OFF.

Setting the <a href="/package/extension5/sspread/properties/editmodereplace">EditModeReplace</a> property, so that all cell contents can be selected when the input mode is turned on.

Setting the <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a> property to $TRUE always turns on the input mode, so the EditMode property is disabled.

***Focus mode and input mode***

The SSpread object must be in focus for the input mode to turn on. Even if this property is set to $TRUE without focus, the input mode will not turn ON.

For example, if the button is clicked by writing the following in the OnTouch event of the Button class, the input mode will not be turned ON. This is because the focus moves to the button when the button is clicked.
```
Button Button1 {
    Function OnTouch(e) {
        ^.SSpread1.EditMode = $TRUE; /* Does not turn ON */
    }
}
```
As shown below, the result is the same even if the focus is set with the <a href="/package/extension5/sspread/methods/setfocus">SetFocus</a>  method immediately before. This is because the focus is not changed when the SetFocus method is called. (The actual focus change is done after the OnTouch event handler ends)
```
Function OnTouch(e) {
    ^.SSpread1.SetFocus();
    ^.SSpread1.EditMode = $TRUE; /* Does not turn ON */
}
```
If you press the key specified in the <a href="/package/standard/button/properties/altkey">Altkey</a> property of the Button class to raise the Touch event, the focus will not move to the button. At this time, if the SSpread object has focus, the input mode will be ON.
```
Button Button1 {
    AltKey = $F06;
    Function OnTouch(e) {
        ^.SSpread1.EditMode = $TRUE; /* Turns on if SSpread has focus */
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a>, <a href="/package/extension5/sspread/properties/editmodereplace">EditModeReplace</a> property<br>
<a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a>, <a href="/package/extension5/sspread/evenst/editmodeoff">EditModeOff</a> event