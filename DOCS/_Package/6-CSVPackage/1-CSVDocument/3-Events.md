---
layout: default

grand_parent: 6. CSV Package
parent: CSVDocument Class
has_children: true
title: Events
nav_order: 3
permalink: /package/csvpackage/csvdocument/events
has_toc: false

---
# {{ page.title }}

Events defined in the CSVDocument class occur in the process of assigning CSV data to an array object by the [[] << CSV constant](/package/csvpackage/csvdocument/operators/1) operator or [[] << CSVDocument](/package/csvpackage/csvdocument/operators/2) operator.

Events defined in the CSVDocument class occur regardless of the type of the object to which they are assigned. Since they are not defined by the object to which they are assigned, these events are displayed in the event view of Biz / Designer. It is not. Write the event handler that handles the events of the CSVDocument class directly in the script editor.

|Name       | Description |
|----------	|-------------|
| [BeginBreak](/package/csvpackage/csvdocument/events/beginbreak) |Occurs when loading keybreak items<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [EndBreak](/package/csvpackage/csvdocument/events/endbreak) |Occurs at the end of loading keybreak items<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [KeyBreak](/package/csvpackage/csvdocument/events/keybreak) |Caused by a key break<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
| [LoadBreak](/package/csvpackage/csvdocument/events/loadbreak) |Occurs when all CSV data assignments are complete|