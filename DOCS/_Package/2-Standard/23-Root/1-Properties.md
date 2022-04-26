---
layout: default

grand_parent: 2. Standard Package
parent: Root Class

title: Properties
nav_order: 1
permalink: /package/standard/root/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Root class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AltKeyPriority](/package/standard/root/properties/altkeypriority) | CRW | integer | 0 | |
|[BgColor](/package/standard/root/properties/bgcolor) | CRW | integer | $STD | |
|[CacheMode](/package/standard/root/properties/cachemode) | CRW | integer | Root.CacheNetwork | |
|[CloseBox](/package/standard/root/properties/closebox) | CRW | boolean | $TRUE | |
|[ControlBox](/package/standard/root/properties/controlbox) | CRW | boolean | $TRUE | |
|[DirectInput](/package/standard/root/properties/directinput) | CRW | boolean | $FALSE | |
|[Embedded](/package/standard/root/properties/embedded) | R | integer |  | |
|[ExtConnection](/package/standard/root/properties/extconnection) | R | boolean |  | |
|[HttpTimeout](/package/standard/root/properties/httptimeout) | CRW | integer | 0 | |
|[Icon](/package/standard/root/properties/icon) | CRW | integer | 0 | |
|[Indicator](/package/standard/root/properties/indicator) | CRW | integer | Root.indAll | |
|[InputTimeout](/package/standard/root/properties/inputtimeout) | CRW | integer | 120 | |
|[MaximizeBox](/package/standard/root/properties/maximizebox) | CRW | boolean | $TRUE | |
|[MinimizeBox](/package/standard/root/properties/minimizebox) | CRW<br>CR<br>**<small>Mobile</small>** | boolean | $TRUE | |
|[ReSize](/package/standard/root/properties/resize) | CRW | integer | $TRUE | |
|[ShellId](/package/standard/root/properties/shellid) | CRW | String |  | |
|[Title](/package/standard/root/properties/title) | CRW | String |  | |
|[TitleBar](/package/standard/root/properties/titlebar) | CRW | boolean | $TRUE | |
|[Value](/package/standard/root/properties/value)* | CRW | String |  | |
|[X](/package/standard/root/properties/x) | CRW | integer |  | |
|[Y](/package/standard/root/properties/y) | CRW | integer |  | |

**<small>Visible property can be specified after Version 4.1.3</small>**

Only available for Mobile version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoDial](/package/standard/root/properties/autodial) | CRW | integer | Root.Up+Root.Down  |             |
|[DialEntry](/package/standard/root/properties/dialentry) | CRW | String |   |         |
|[HttpRetryTime](/package/standard/root/properties/httpretrytime) | CRW | integer | 0  ||
|[UseHttpPreconfig](/package/standard/root/properties/usehttppreconfig) | CRW | boolean | $TRUE  |             |

Only available for Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[ReloggedIn](/package/standard/root/properties/reloggedin) | R | boolean | $FALSE  |             |
|[ScrollBarSize](/package/standard/root/properties/scrollbarsize) | CR | integer |  16  |         |
|[BackKeyMode](/package/standard/root/properties/backkeymode) | CRW | integer | Root.ConfirmClose+Root.RaiseKeyDown  ||

Only available for both Mobile and Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[DisplayOrient](/package/standard/root/properties/displayorient) | CRW | integer | Root.deg0<br>**<small>Root.UNSPECIFIED in AI</small>**  |             |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
