---
layout: default

grand_parent: Form Class
parent: Events
has_children: false
title: Form.KeyDown Event
nav_order: 5
permalink: /package/standard/form/events/keydown
---
# {{ page.title }}


The KeyDown event is triggered by pressing the keyboard. By processing the KeyDown event in the OnKeyDown event handler, you can express the behavior like an accelerator.

 

The following child objects are attached to the Event object.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4erg{border-color:inherit;font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-6t3r{font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-f7v4">Type</th>
    <th class="tg-f7v4">Name</th>
    <th class="tg-f7v4">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">ShiftKey</td>
    <td class="tg-0pky">1 if the Shift key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">CtrlKeyKey</td>
    <td class="tg-0pky">1 if the Ctrl key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">AltKey</td>
    <td class="tg-0pky">1 if the Alt key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0lax">String</td>
    <td class="tg-6t3r">Key</td>
    <td class="tg-0lax">Pressed key<br>See the table below for special keys.</td>
  </tr>
</tbody>
</table>

Example of use
```
Function OnKeyDown(e) {
    if (e.CtrlKey == 1 && e.Key == "G") {
        /* Ctrl+Gを押したときForm2に画面を切り替えます */
        //.Form1.Delete();
        //.Get("Form2.crs");
    }
}
 
 ```

 <br><br>

***Value stored in the Key object (special key)***


<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-f8tv{border-color:inherit;font-style:italic;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-8zwo{font-style:italic;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-f7v4">Key Type</th>
    <th class="tg-f7v4">Stored Value</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Esc</td>
    <td class="tg-f8tv">"ESCAPE"</td>
  </tr>
  <tr>
    <td class="tg-0pky">BackSpace</td>
    <td class="tg-f8tv">"BACK"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Tab</td>
    <td class="tg-8zwo">"TAB"</td>
  </tr>
  <tr>
    <td class="tg-0lax">ENTER</td>
    <td class="tg-0lax">"RETURN"</td>
  </tr>
  <tr>
    <td class="tg-0lax">change</td>
    <td class="tg-0lax">"CONVERT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">No conversion</td>
    <td class="tg-0lax">"NONCONVERT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Space</td>
    <td class="tg-0lax">"SPACE"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Insert. Insert.</td>
    <td class="tg-0lax">"INSERT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Home</td>
    <td class="tg-0lax">"HOME"</td>
  </tr>
  <tr>
    <td class="tg-0lax">PageUp</td>
    <td class="tg-0lax">"PRIOR"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Delete</td>
    <td class="tg-0lax">"DELETE"</td>
  </tr>
  <tr>
    <td class="tg-0lax">End</td>
    <td class="tg-0lax">"END"</td>
  </tr>
  <tr>
    <td class="tg-0lax">PageDown</td>
    <td class="tg-0lax">"NEXT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Direction key left</td>
    <td class="tg-0lax">"LEFT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">On the arrow keys</td>
    <td class="tg-0lax">"UP"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Direction key right</td>
    <td class="tg-0lax">"RIGHT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Down arrow keys</td>
    <td class="tg-0lax">"DOWN"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Pause Break</td>
    <td class="tg-0lax">"PAUSE"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Left Windows key</td>
    <td class="tg-0lax">"LWIN"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Right Windows key</td>
    <td class="tg-0lax">"RWIN"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad 0-9 _</td>
    <td class="tg-0lax">"NUMPAD0" to "NUMPAD9"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad.</td>
    <td class="tg-0lax">"DECIMAL"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad *</td>
    <td class="tg-0lax">"MULTIPLY"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad +</td>
    <td class="tg-0lax">"ADD"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad /</td>
    <td class="tg-0lax">"DIVIDE"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Numeric keypad-</td>
    <td class="tg-0lax">"SUBTRACT"</td>
  </tr>
  <tr>
    <td class="tg-0lax">NumLock</td>
    <td class="tg-0lax">"NUMLOCK"</td>
  </tr>
  <tr>
    <td class="tg-0lax">F1 ~ F24</td>
    <td class="tg-0lax">"F1" - "F24"</td>
  </tr>
  <tr>
    <td class="tg-0lax">Scroll Lock</td>
    <td class="tg-0lax">"SCROLL"</td>
  </tr>
</tbody>
</table>
For the KeyDown event, the type of key operation that occurs and the object that is the source of the event are determined by which object the keyboard focus is on in the Biz / Browser screen.

 

The source object for the KeyDown event is the Form object in which the object is located, if the object has keyboard focus. If the keyboard focus is not on any object, it originates from the top Form object.
<br><br>

***Priority order for key operations***

When multiple meanings are assigned to one key operation and the key operation is actually performed, the priority order of execution is as follows.

<br><br>
1. For key operations set in the Tab key, Shift + Tab key, NextTabKey property, and PrevTabKey property, focus movement is performed preferentially.

2. Object-specific key operations are performed.

3. The key operation assigned to the AltKey property of the Button object is executed.

4. The KeyDown event is raised.

<br>

* The operation that occurs in one key operation is one of focus movement, object-specific operation, AltKey property operation, and KeyDown event issuance.

<br><br>

***Precautions when using the KeyDown event***

- It is recommended not to use special keys (Kanji, no conversion, BackSpace , etc.) used for character input in the KeyDown event because they are strongly affected by the type of IME and the state of the object.

 

- It is recommended not to use the same key as the system key (system menu Alt + Space , window switching Alt + Tab , etc.) as it may cause confusion in operability.

 

- It is recommended that you do not use keys that have unique meanings, such as PrintScreen and Pause , as they can cause confusion.

 

- The KeyDown event occurs for key operations recognized by Windows . Windows keystroke recognition is affected by keyboard hardware. For example, there is a model in which the NumLock key and the ScrollLock key are used together with one button and selected with the Shift key. Shift + ScrollLock does not occur on these keyboards .

 

- Depending on the model, special keys such as Pause and NumLock may be recognized as different keys when pressed at the same time as the Ctrl , Shift , and Alt keys. When using these special keys, make sure that the KeyDown event is fired correctly on the keyboard you are actually using .

 

- The KeyDown event may not occur depending on the type of object that is focused on the key press.

<br><br>

***Restrictions on Android version***


In the Android version, there are restrictions on the objects that generate key events and the keys that can be used.

For details , refer to the <a href="/bizBrowserV/2/2-5/">Android Version Features and Restrictions</a>.














