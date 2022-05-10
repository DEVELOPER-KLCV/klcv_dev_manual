---
layout: default

grand_parent: 6. CSV Package
parent: CSVDocument Class
title: CSV Constants
nav_order: 5
permalink: /package/csvpackage/csvdocument/csvcontants
has_toc: false
---
# {{ page.title }}

The CSVDocument class defines CSV constants. CSV constants can be used to set data by the [[] << CSV constant](/package/csvpackage/csvdocument/operators/1) operator, [CSVDocument << CSV constant](/package/csvpackage/csvdocument/operators/5) operator.

CSV constant blocks are not grammatically related to CRS scripts, so CRS syntax (such as enclosing strings in ""), constants (such as $ RED), operators (such as + and-), and functions. Etc. cannot be used. You have to follow the format as CSV.

The CSV format is as follows.

1. The number of columns should be constant. However, if the number of columns does not match except for the first row, it will be complemented so that the number of columns is the same as the first row.

1. Columns are separated by commas that are not escaped.

1. Lines are separated by unescaped line breaks.

1. If the data contains commas or line breaks, use "(double quotation) to enclose and escape the data.

1. If you want to include "(double quotation) itself in the data enclosed in" (double quotation), describe two consecutive data like "".

Example
```
var csvdata = new CSVDocument;
csvdata << CSV {
A,1200,3000,100,C,XX1
A,1200,3000,100,C,XX1
A,1200,3000,100,C,XX1
    :
};
```

You can write CSV data directly in the CRS script in the following format.

```
CSV {
列1,列２,列３
列1,列２,列３
列1,列２,列３
列1,列２,列３
    :
};
```

CSV constants can be named for columns.

Named CSV constant
```
CSV( name1, name2, name3 ) {
列1,列２,列３
列1,列２,列３
列1,列２,列３
列1,列２,列３
    :
};
```

The added column name can be obtained by the [GetColumnName](/package/csvpackage/csvdocument/methods/getcolumnname) method and can be changed by the [SetColumnName](/package/csvpackage/csvdocument/methods/setcolumnname) method.

In addition to simply using the column name as a name, it can represent an object name or property name. When copying to an array with the [[ ] << CSV constant](/package/csvpackage/csvdocument/operators/1) operator, explicitly specify the object or property to copy to. I can do it.