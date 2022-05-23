---
layout: default

parent: 2. Standard Package
has_children: true

title: FocusOperationEvent Class
nav_order: 11
permalink: /package/standard/focusoperationevent

---

# {{ page.title }}

<a href="/img/Package/Standard-FocusOperationEvent.PNG" target="_blank">
<img src="/img/Package/Standard-FocusOperationEvent.PNG" alt="login image"></a>

The class used to notify the <a href="/package/standard/focusobject/events/focusoperation">FocusOperation</a> event of the <a href="/package/standard/focusobject">FocusObject</a> class.


The FocusOperation event is fired when an operation that causes the focus to move while the object is in keyboard focus. The operation to move the focus is the operation to press the TAB key or the <a href="/package/standard/focusobject/properties/nexttabkey">NextTabKey</a>, the key set in the <a href="/package/standard/focusobject/properties/prevtabkey">PrevTabKey</a> property, and the operation to execute AutoTab for the class with the AutoTab property. The FocusOperation event does not occur for operations other than these.


The FocusOperation event occurs exclusively with focus movement, as specified by the <a href="/package/standard/focusobject/properties/autotabfocus">FocusObject.AutoTabFocus</a> property, which directs automatic focus movement. If the AutoTabFocus property is $ TRUE, the operation that causes the focus move will move the focus and the FocusOperation event will not be fired. Conversely, if the AutoTabFocus property is $ FALSE, the Focus will not move and the FocusOperation event will be fired.


By using the FocusObject's <a href="/package/standard/focusobject/properties/autotabfocus">AutoTabFocus</a> property,  <a href="/package/standard/focusoperationevent">FocusOperation</a> event, <a href="/package/standard/focusobject/methods/movefocus">MoveFocus</a> method, and FocusOperationEvent object in combination, application-specific actions such as checking the input value can be intervened in the focus movement action by the Tab key or Enter key. As shown in the example below, if the input value is empty, an error message is displayed without moving the focus, and if the input value is valid, the focus is moved to the next object.

Example
```
TextBox tx {
    :
    AutoTabFocus = $FALSE;
    :
    Function OnFocusOperation(e) {
        if( value == "" ) {
            BgColor = $RED;
            MessageBox("入力してください");
            return;
        }
        BgColor = $STD;
        MoveFocus(e.Direction);
    }
}
```

**Default properties and ValueType**
 

The default property is <a href="/package/system/event/properties/reason">Reason</a>. The ValueType specification is invalid.


**Handling of Focus Operation events in the Mobile version** 

The FocusOperationEvent class does not exist in the Mobile version, but it is designed so that it can be treated in the same way as an Event object with a Key and Direction object attached.