---
layout: default

grand_parent: Exception Class
parent: Properties
has_children: false
title: Exception.SourceOffset property
nav_order: 4
permalink: /package/system/exception/properties/SourceOffset
---
# {{ page.title }}

The execution position of the CRS script that caused the exception is indicated by the byte position from the beginning.

This property is read-only and cannot be changed. It is set automatically when passed to the throw statement.

※ Effective only when debugging from Biz / Designer to prevent performance degradation during execution.