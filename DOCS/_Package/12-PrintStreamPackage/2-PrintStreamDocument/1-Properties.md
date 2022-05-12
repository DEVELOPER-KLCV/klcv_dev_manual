---
layout: default

grand_parent: 
parent: 12. PrintStream Package
has_children: true

parent: PrintStreamDocument Class
has_children: true
title: Properties
nav_order: 1
permalink: /package/printstreampackage/printstreamdocument/properties
has_toc: false
---
# {{ page.title }}

The following properties are defined in the PrintStreamDocument class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|-------------|------|
|[Height](/package/printstreampackage/printstreamdocument/properties/height) | CRW | integer | 0 | |
|[ImagePrint](/package/printstreampackage/printstreamdocument/properties/imageprint) | CRW | integer | 1 | |
|[MarginLeft](/package/printstreampackage/printstreamdocument/properties/marginleft) | CRW | Number | 0 | |
|[MarginTop](/package/printstreampackage/printstreamdocument/properties/margintop) | CRW | Number | 0 | |
|[Orientation](/package/printstreampackage/printstreamdocument/properties/orientation) | CRW | integer | $VERTICAL | |
|[PaperSize](/package/printstreampackage/printstreamdocument/properties/papersize) | CRW | String | 9 | |
|[Printer](/package/printstreampackage/printstreamdocument/properties/printer) | R | String | PrintStream value | |
|[StoragePlace](/package/printstreampackage/printstreamdocument/properties/storageplace) | CR | integer | $FILE | |
|[Width](/package/printstreampackage/printstreamdocument/properties/width) | CRW | integer | 0 | |
|[ZoomHeight](/package/printstreampackage/printstreamdocument/properties/zoomheight) | CRW | Number | 0 | |
|[ZoomMatchsize](/package/printstreampackage/printstreamdocument/properties/zoommatchsize) | CRW | integer | 0 | |
|[ZoomWidth](/package/printstreampackage/printstreamdocument/properties/zoomwidth) | CRW | Number | 0 | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

**Overwriting property values ​​when printing definition information is read**

This information records the paper size, paper orientation, and margin adjustments, which overwrite the properties [PaperSize](/package/printstreampackage/printstreamdocument/properties/papersize), [Orientation](/package/printstreampackage/printstreamdocument/properties/orientation), [Height](/package/printstreampackage/printstreamdocument/properties/height), [Width](/package/printstreampackage/printstreamdocument/properties/width), [MarginLeft](/package/printstreampackage/printstreamdocument/properties/marginleft), and [MarginTop](/package/printstreampackage/printstreamdocument/properties/margintop).

Once this PSS file is printed with PrintStream for Internet Explorer, the registry records the printer name, margin adjustment, print size adjustment, and whether or not to print an image. In Biz / Browser, if this record is present, the properties [Printer](/package/printstreampackage/printstreamdocument/properties/printer), [ImagePrint](/package/printstreampackage/printstreamdocument/properties/imageprint), [MarginLeft](/package/printstreampackage/printstreamdocument/properties/marginleft), [MarginTop](/package/printstreampackage/printstreamdocument/properties/margintop), [ZoomMatchsize](/package/printstreampackage/printstreamdocument/properties/zoommatchsize), [ZoomHeight](/package/printstreampackage/printstreamdocument/properties/zoomheight), and [ZoomWidth](/package/printstreampackage/printstreamdocument/properties/zoomwidth) will be overwritten.

Therefore, when using a unique value in Biz / Browser, set it after reading the print definition information (after acquiring the return value ret.from = 0 of the [Extract](/package/printstreampackage/printstreamdocument/methods/extract) method).