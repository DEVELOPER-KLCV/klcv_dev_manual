---
layout: default

grand_parent: 2. Standard Package
parent: FocusObject Class

title: Properties
nav_order: 1
permalink: /package/standard/focusobject/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FocusObject class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[AutoTabFocus](/package/standard/focusobject/properties/autotabfocus) | CRW | boolean | $TRUE | Control of focus movement by key operation<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12"> |
|[NextTabKey](/package/standard/focusobject/properties/nexttabkey) | CRW | integer | $STD | Keys to move keyboard focus to the next object<br>It is now possible to specify $ END and $ S_END since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add400.gif" alt="Image" width="50" height="12"> <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12">.<br>There are limits in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> |
|[PrevTabKey](/package/standard/focusobject/properties/prevtabkey) | CRW | integer | $STD | Keys to move keyboard focus to the previous object<br>Since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add400.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12"> it is now possible to specify $ END and $ S_END .<br>There are limits in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> |
|[SkipTabFocus](/package/standard/focusobject/properties/skiptabfocus) | CRW | boolean | $FALSE | Suppression of focus acceptance by key operation<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12"> |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable