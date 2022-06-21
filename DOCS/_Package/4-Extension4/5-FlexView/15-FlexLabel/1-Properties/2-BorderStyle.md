---
layout: default

grand_parent: FlexLabel Class
parent: Properties
has_children: false
title: BorderStyle Property
nav_order: 2
permalink: /package/extension4/flexview/flexlabel/properties/borderstyle
---
# {{ page.title }}

Specify the border type. Only valid if the <a href="/package/extension4/flexview/flexcheckbutton/properties/border">Border</a> property is $TRUE.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-i7zr">$SUNKEN</td>
    <td class="tg-tcrt">0</td>
    <td class="tg-i7zr">The whole is displayed in a concave shape</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$RISED</td>
    <td class="tg-tcrt">1</td>
    <td class="tg-i7zr">The whole is displayed in a convex shape</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ETCHED</td>
    <td class="tg-tcrt">2</td>
    <td class="tg-i7zr">The border is displayed in a concave shape.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$BUMP</td>
    <td class="tg-tcrt">3</td>
    <td class="tg-i7zr">Displays the border in a convex shape</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$GRAYFRAME</td>
    <td class="tg-tcrt">4</td>
    <td class="tg-i7zr">Shows a border in two colors of gray</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$SOFT</td>
    <td class="tg-tcrt">5</td>
    <td class="tg-i7zr">Display the frame in black and white</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$SOFTETCHED</td>
    <td class="tg-tcrt">6</td>
    <td class="tg-i7zr">The border is displayed in a soft concave shape.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$SOFTBUMP</td>
    <td class="tg-tcrt">7</td>
    <td class="tg-i7zr">The border is displayed in a soft convex shape.</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$PLANE</td>
    <td class="tg-tcrt">8</td>
    <td class="tg-i7zr">Display with a single black line</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$DASH</td>
    <td class="tg-tcrt">9</td>
    <td class="tg-i7zr">Display with a long dotted line<br>On <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"># it will be the same display as $DOT</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$DOT</td>
    <td class="tg-tcrt">10</td>
    <td class="tg-i7zr">Display with a fine dotted line</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$FLATSUNKEN</td>
    <td class="tg-tcrt">11</td>
    <td class="tg-i7zr">Displays the whole with a low concave shape</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$FLATRISED</td>
    <td class="tg-tcrt">12</td>
    <td class="tg-i7zr">Display the whole with a low convex shape</td>
  </tr>
</tbody>
</table>


Example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/base/base1-23.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>
