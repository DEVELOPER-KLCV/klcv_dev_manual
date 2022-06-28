---
layout: default

grand_parent: ImageList Class
parent: Properties
has_children: false
title: ImageList.MaskUse Property
nav_order: 8
permalink: /package/extension4/imagelist/properties/maskuse
---
# {{ page.title }}

Specify $ TRUE for image transparency processing.

The part of the color specified by <a href="/package/extension4/imagelist/properties/maskcolr">MaskColR</a>, <a href="/package/extension4/imagelist/properties/maskcolg">MaskColG</a>, and <a href="/package/extension4/imagelist/properties/maskcolb">MaskColB</a> becomes the transparent color.

For example,

MaskUse = $ TRUE;
MaskColR = 255;
MaskColG = 0;
MaskColB = 0;

Then, the red part of the image becomes a transparent color, and it becomes transparent instead of being displayed in red.

Use PNG format for images that want to use transparent colors. Due to the characteristics of the image, the JPEG format cannot make the transparent part one color.