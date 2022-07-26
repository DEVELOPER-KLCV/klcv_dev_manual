---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ProcessDelete Property
nav_order: 82
permalink: /package/extension5/sspread/properties/processdelete
---
# {{ page.title }}

Set whether to delete the data or formula in the selected cell with the Delete key.

Specify $DeleteDataOnly to delete only the data in the cell, and $DeleteAll to delete the formula set in the cell as well. The initial value is $DeleteNone (Delete key is invalid).

The EditError event is raised if any of the selected cells have a locked cell. 

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Related Item<br>
<a href="/package/extension5/sspread/events/editerror">EditError</a> event