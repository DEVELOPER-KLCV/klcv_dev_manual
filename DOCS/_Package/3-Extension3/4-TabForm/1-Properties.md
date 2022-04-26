---
layout: default

grand_parent: 3. Extension3 Package
parent: TabForm Class

title: Properties
nav_order: 1
permalink: /package/extension3/TabForm/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TabForm class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[Height](/package/extension3/TabForm/properties/height) | R | integer |  | |
|[Selected](/package/extension3/TabForm/properties/selected) | CRW | boolean |  | |
|[TabBgColor](/package/extension3/TabForm/properties/TabBgColor) | CRW | integer | $STD | |
|[TabFgColor](/package/extension3/TabForm/properties/TabFgColor) | CRW | integer | $STD | |
|[Title](/package/extension3/TabForm/properties/Title) | CRW | String<br>UString(※) |  | |
|[Width](/package/extension3/TabForm/properties/width) | R | integer |  | |
|[X](/package/extension3/TabForm/properties/x) | R | integer |  | |
|[Y](/package/extension3/TabForm/properties/y) | R | integer |  | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

※ The [HorizontalScale](), [VerticalScale](), and [FontScale]() properties of the Form class are not inherited by this class. If you want to use these features, place the Form inside the TabForm.
 
