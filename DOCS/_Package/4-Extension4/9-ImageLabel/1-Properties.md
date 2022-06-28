---
layout: default

grand_parent: 4. Extension4 Package
parent: ImageLabel Class

title: Properties
nav_order: 1
permalink: /package/extension4/imagelabel/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ImageLabel class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[BoxStyle](/package/extension4/imagelabel/properties/boxstyle) | CRW | integer | $BOX |Label border style |
|[HorzPlacement](/package/extension4/imagelabel/properties/horzplacement) | CRW | integer | $STD | Horizontal display position of images and texts|
|[ImageHeight](/package/extension4/imagelabel/properties/imageheight) | CRW | integer | 32 |Height when enlarging/ reducing the image |
|[ImageWidth](/package/extension4/imagelabel/properties/imagewidth) | CRW | integer | 32 |Width when enlarging / reducing the image |
|[NoPrefix](/package/extension4/imagelabel/properties/noprefix) | CRW | boolean | $FALSE |Mode without interpretation of & <br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[Resize](/package/extension4/imagelabel/properties/resize) | CRW | integer | $STD | How to enlarge / reduce the image |
|[Spacing](/package/extension4/imagelabel/properties/spacing) | CRW | integer | 0 |Peripheral margin|
|[TextAlign](/package/extension4/imagelabel/properties/textalign) | CRW | integer | $STD | Display position in the text display area <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[VertPlacement](/package/extension4/imagelabel/properties/vertplacement) | CRW | integer | $STD | Vertical display position of images and texts|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable