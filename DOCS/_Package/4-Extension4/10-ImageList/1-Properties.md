---
layout: default

grand_parent: 4. Extension4 Package
parent: ImageList Class

title: Properties
nav_order: 1
permalink: /package/extension4/imagelist/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

 
# {{ page.title }}

The following properties are defined in the ImageList class.

| Name       | Access | Type    | Initial Value | Description                                        |
|------------|--------|---------|:-------------:|----------------------------------------------------|
| [IconCount](/package/extension4/imagelist/properties/iconcount) | R      | integer |       0       | Total number of loaded images                      |
| [IcoHeight](/package/extension4/imagelist/properties/iconheight) | CRW    | integer |       16      | The height of the image included in the image list |
| [IconWidth](/package/extension4/imagelist/properties/iconwidth)  | CRW    | integer |       16      | The width of the image in the image list           |
| [LargeImage](/package/extension4/imagelist/properties/largeimage) | CRW    | integer |     $FALSE    | LoadIcon method icon type                          |
| [MaskColR](/package/extension4/imagelist/properties/maskcolr)   | CRW    | integer |       0       | Value of red component of transparent color        |
| [MaskColG](/package/extension4/imagelist/properties/maskcolg)   | CRW    | integer |       0       | Value of green component of transparent color      |
| [MaskColB](/package/extension4/imagelist/properties/maskcolb)   | CRW    | integer |       0       | Value of blue component of transparent color       |
| [MaskUse](/package/extension4/imagelist/properties/maskuse)    | CRW    | boolean |     $FALSE    | Use of image transparency                          | 