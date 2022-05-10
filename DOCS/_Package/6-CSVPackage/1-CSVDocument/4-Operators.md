---
layout: default

grand_parent: 6. CSV Package
parent: CSVDocument Class
has_children: true
title: Operators
nav_order: 4
permalink: /package/csvpackage/csvdocument/operators
has_toc: false
---
# {{ page.title }}

The CSVDocument class defines the following operators that support [CSV constants](/package/csvpackage/csvdocument/csvcontants) and arrays.

|Name       | Description |
|----------	|-------------|
|[[ ] << CSV constants](/package/csvpackage/csvdocument/operators/1) | Load the CSV constant on the right side into the array object on the left side |
| [[ ] << CSVDocument](/package/csvpackage/csvdocument/operators/2) | Load the CSVDocument data on the right side into the array object on the left side |
| [CSVDocument << CSVDocument](/package/csvpackage/csvdocument/operators/3) | Loads the data of the CSVDocument object on the right side into the CSVDocument object on the left side |
|[CSVDocument << [ ]](/package/csvpackage/csvdocument/operators/4) | Loads the data of the array object on the right side into the CSVDocument object on the left side |
|[CSVDocument << CSV constants](/package/csvpackage/csvdocument/operators/5) |  Load the CSV constant on the right side into the CSVDocument object on the left side |