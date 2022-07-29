---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ShadowLight Property
nav_order: 122
permalink: /package/extension5/sspread/properties/shadowlight
---
# {{ page.title }}

Sets the color of row and column headers and the uneven light areas of label cells.

For row and column headers, this is only valid if the <a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a> property is $AppearanceStyleClassic.
For label cells, this is valid only when either the<a href="/package/extension5/sspread/properties/typetextshadow">TypeTextShadow</a> property or the <a href="/package/extension5/sspread/properties/typetextshadowin">TypeTextShadowIn</a> property is $TRUE (3D display).

Specify a <a href="/base/color">color constant</a> and
<a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>.
The initial value is $STD (system standard color).

<small><span style="color:red">Added since Ver.5.0.1</span></small>

***Header color setting property***

ShadowLight ↓　<br>
<a href="/img/Package/Ext5-SSpread-ShadowDark.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread-ShadowDark.PNG" alt="login image">
</a> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <a href="/package/extension5/sspread/properties/shadowdark">ShadowDark</a> ↑


Example of usage<br>
```
AppearanceStyle = $AppearanceStyleClassic;
ShadowColor = $DCYAN;
ShadowText = $WHITE;
ShadowLight = "#DAEAD0";
ShadowDark = "#005C50";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a>, <a href="/package/extension5/sspread/properties/shadowcolor">ShadowColor</a>, <a href="/package/extension5/sspread/properties/shadowdark">ShadowDark</a>, <a href="/package/extension5/sspread/properties/shadowtext">ShadowText</a>,  <a href="/package/extension5/sspread/properties/typetextshadow">TypeTextShadow</a>, <a href="/package/extension5/sspread/properties/typetextshadowin">TypeTextShadowIn</a> properties  