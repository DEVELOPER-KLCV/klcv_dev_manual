---
layout: default

grand_parent: 9. HTTP Package
parent: HttpDownload Class
has_children: true
title: Properties
nav_order: 1
permalink: /package/httppackage/httpdownload/properties
has_toc: false
---
# {{ page.title }}

The following properties are defined in the HttpDownload class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|-------------|---------|
| [Retry](/package/httppackage/httpdownload/properties/retry) | CRW      |integer | 3 | Number of retries|
| [RetryWait](/package/httppackage/httpdownload/properties/retrywait) | CRW      |integer | 5 | Waiting time for retry |
| [Wait](/package/httppackage/httpdownload/properties/wait) | CRW      |integer | 5 | Waiting time for the next download |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable