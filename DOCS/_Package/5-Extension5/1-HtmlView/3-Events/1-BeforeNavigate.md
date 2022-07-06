---
layout: default

grand_parent: HtmlView Class
parent: Events
has_children: false
title: HtmlView.BeforeNavigate Event
nav_order: 1
permalink: /package/extension5/htmlview/events/beforenavigate
---
# {{ page.title }}

Occurs when trying to move to a specified URL.

If $TRUE is returned, movement is permitted, and $FALSE is canceled.

The special event handler stops executing the script until it returns from the event handler.

Also, operations involving the GUI cannot be performed within this event handler.

The following child objects are attached to the Event object.

| Type   | Name | Description                |
|:--------:|:------:|:----------------------------:|
| String | **_url_**  | URL you are trying to move |