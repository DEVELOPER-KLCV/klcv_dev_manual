---
layout: default

grand_parent: Dialog Class
parent: Events
has_children: false
title: Dialog.WindowStateChanged Event
nav_order: 3
permalink: /package/standard/dialog/events/windowstatechanged
---
# {{ page.title }}

Occurs when a state change occurs, such as maximizing or minimizing a dialog.

The following child objects are attached to the Event object.

<table>
    <tr>
        <td>Type</td>
        <td>Name</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>Number</td>
        <td>state</td>
        <td>The following values ​​are set.
        <table>
                <tr>
                    <td>Constant</td>
                    <td>Value</td>
                    <td>Description</td>
                </tr>
                <tr>
                    <td>$MINIMIZE</td>
                    <td>1</td>
                    <td>Minimize</td>
                </tr>
                <tr>
                    <td>$MAXIMIZE</td>
                    <td>2</td>
                    <td>Maximize</td>
                </tr>
                <tr>
                    <td>$RESTORE</td>
                    <td>3</td>
                    <td>When the size is other than maximize / minimize</td>
                </tr>
            </table>
        </td>
    </tr>
</table>

<br>**<small>Added since Version 4.1.3</small>**
<br>**<small>Not supported in Mobile, AI</small>**