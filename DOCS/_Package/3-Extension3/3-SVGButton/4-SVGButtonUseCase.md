---
layout: default

grand_parent: 3. Extension3 Package
parent: SVGButton Class

title: Example of using SVGButton
nav_order: 4
permalink: /package/extension3/svgbutton/example

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

```
Form Form1 {
    X = 0;
    Y = 0;
    Width = 400;
    Height = 300;
    XmlDocument svg << xml <<-
    <?xml version="1.0" encoding="Shift_JIS"?>
    <!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.0//EN"
    "http://www.w3.org/TR/2001/REC-SVG-20010904/DTD/svg10.dtd">
    <svg xmlns="http://www.w3.org/2000/svg">
    <defs>
    <linearGradient id="blue-neon" x1="0%" y1="0%" x2="100%" y2="0%"
        spreadMethod="pad" gradientUnits="objectBoundingBox">
    <stop offset="0%" style="stop-color:rgb(0,128,128);stop-opacity:1"/>
    <stop offset="10%" style="stop-color:rgb(0,255,255);stop-opacity:1"/>
    <stop offset="50%" style="stop-color:rgb(255,255,255);stop-opacity:1"/>
    <stop offset="90%" style="stop-color:rgb(0,255,255);stop-opacity:0.75"/>
    <stop offset="100%" style="stop-color:rgb(0,192,192);stop-opacity:1"/>
    </linearGradient>
    </defs>
    <ellipse cx="72" cy="32" rx="70" ry="30" fill="url(#blue-neon)"/>
    <text x="15" y="40"
        style="fill:rgb(202,36,145);font-size:24px">SVGButton</text>
    </svg>
    ->>;
    SVGButton SVGButton1 {
        X = 20;
        Y = 40;
        Width = 144;
        Height = 64;
        Image = Form1.svg;
    }
}
```