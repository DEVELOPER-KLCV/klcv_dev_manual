---
layout: default

grand_parent: HtmlView Class
parent: Properties
has_children: false
title: HtmlView.AllowAction Property
nav_order: 2
permalink: /package/extension5/htmlview/properties/allowaction
---
# {{ page.title }}

Specifies the actions to allow.

If specify more than one, combine them with the "+" operator.

| Constant       | Value | Description                                                   |
|----------------|:-----:|---------------------------------------------------------------|
| $ALLOW_NONE    |   0   | The following operations are not allowed                      |
| $ALLOW_SCRIPT  |   1   | Allow scripts                                                 |
| $ALLOW_JAVA    |   2   | Allow Java                                                    |
| $ALLOW_ACTIVEX |   4   | Allow ActiveX                                                 |
| $ALLOW_POPUP   |   8   | Allow pop-up display by <a target=”_blank”> or window.open () <br><small><span style="color:red">Added since Ver.5.0.3</span></small> |