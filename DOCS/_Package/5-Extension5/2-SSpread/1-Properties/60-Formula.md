---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Formula Property
nav_order: 60
permalink: /package/extension5/sspread/properties/formula
---
# {{ page.title }}

Set the formula in the cell.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string.

Formulas are set by combining cell references, operators, and functions.

There are two types of cell reference styles available for cell references: absolute references and relative references. The cell reference style can be set with the <a href="/package/extension5/sspread/methods/setrefstyle">SetRefStyle</a> method.

No need to specify equals (=) at the beginning of the formula.

Make the cell a data type that can handle the number, in order to display a number as a result of a formula. The same applies when treat the referenced cell used in the formula as a number. Set the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property of the target cell to $CellTypeCurrency (currency type), $CellTypeNumber (numeric type), $ ellTypePercent (percentage type), and $CellTypeScientific (exponential type).

Set the <a href="/package/extension5/sspread/properties/allowuserformulas">AllowUserFormulas</a> property to enter the formula directly on the spreadsheet.

The automatic recalculation of formulas is set with the <a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a> property, <a href="/package/extension5/sspread/methods/recalc">ReCalc</a>, and <a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> methods.

The automatic update of cell references is set in the <a href="/package/extension5/sspread/properties/formulasync">FormulaSync</a> property.

Example of usage<br>
```
Col = 1;
Row = 1;
CellType = $CellTypeNumber;
Value = 1;
 
Col = 2;
Row = 1;
CellType = $CellTypeNumber;
Value = 2;
 
Col = 3;
Row = 1;
CellType = $CellTypeNumber;
Formula = "A1+B1";
 
Col = 4;
Row = 1;
CellType = $CellTypeNumber;
Formula = "SUM(A1, B1, C1)";
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allowuserformulas">AllowUserFormulas</a>, <a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a>, <a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/formulasync">FormulaSync</a> properties<br>
<a href="/package/extension5/sspread/methods/getrefstyle">GetRefStyle</a>, <a href="/package/extension5/sspread/methods/setrefstyle">SetRefStyle</a>, <a href="/package/extension5/sspread/methods/isformulavalid">IsFormulaValid</a>, <a href="/package/extension5/sspread/methods/recalc">ReCalc</a>, <a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> methods


### Predefined functions

The following predefined functions can be used in formulas.

Math / trigonometric functions

| Format                                            | Return value    | explanation                                                                    |
|---------------------------------------------------|-----------------|--------------------------------------------------------------------------------|
| ABS ( ***numerical value*** )                      | Numerical value | Absolute value of the ***numerical value***                                                   |
| ACOS ( ***numerical value*** )                          | Numerical value | Numeric arccosine                                                              |
| ACOSH ( ***numerical value*** )                         | Numerical value | Numeric hyperbolic inverse cosine (inverse function of hyperbolic cosine)      |
| ADD ( ***number 1, number 2*** )                       | Numerical value | Addition of number 1 and number 2                                              |
| ASIN ( ***numerical value*** )                          | Numerical value | Numeric arcsine                                                                |
| ASINH ( ***numerical value*** )                         | Numerical value | Numeric hyperbolic inverse sine (inverse function of hyperbolic sine)          |
| ATAN ( ***numerical value*** )                          | Numerical value | Numerical arctangent                                                           |
| ATAN2 ( ***x coordinate, y coordinate*** )             | Numerical value | x - coordinate - y - coordinate arctangent                                     |
| ATANH ( ***numerical value*** )                         | Numerical value | Hyperbolic tangent of numerical value (inverse function of hyperbolic tangent) |
| CEILING ( ***numerical value, reference value*** )     | Numerical value | Round up tothe nearest multiple of the reference value                         |
| COMBIN ( ***total number, number*** )                  | Numerical value | Number of combinations when selecting the number from the total number         |
| COS ( ***numerical value*** )                           | Numerical value | Numerical cosine                                                               |
| COSH ( ***numerical value*** )                          | Numerical value | Numerical hyperbolic cosine (hyperbolic cosine)                                |
| DEGREES ( ***angle*** )                                 | Numerical value | Convert angles (radians) to degrees                                            |
| EVEN ( ***numerical value*** )                          | Numerical value | Round up the number to the nearest even                                        |
| EXP ( ***numerical value*** )                           | Numerical value | Exponentiation of a number with e as the base                                  |
| FACT ( ***numerical value*** )                          | Numerical value | Factorial of numbers                                                           |
| FLOOR ( ***numerical value, reference value*** )       | Numerical value | Rounds down tothe nearest multiple of the reference value                      |
| INT ( ***numerical value*** )                           | Numerical value | Truncate the number to the nearest integer                                     |
| INVERSE ( ***numerical value*** )                       | Numerical value | Reciprocal of the number ( 1 / number )                                        |
| LN ( ***numerical value*** )                            | Numerical value | Natural logarithm of numbers                                                   |
| LOG ( ***number, x*** )                                | Numerical value | Logarithm of numbers based on x                                                |
| LOG10 ( ***numerical value*** )                         | Numerical value | Logarithm of numbers with base 10                                              |
| MOD ( ***number, divisor*** )                          | Numerical value | Remainder when a number is divided by a divisor                                |
| NEG ( ***numerical value*** )                           | Numerical value | Convert the code of a number                                                   |
| ODD ( ***numerical value*** )                           | Numerical value | Round up the number to the nearest odd number                                  |
| PI ()                                             | Numerical value | Pi ( 3.1415926536 )                                                            |
| POWER ( ***numerical value, index*** )                 | Numerical value | Exponentiation of thebase of the number                                        |
| PRODUCT ( ***number 1, number 2, ...***)              | Numerical value | Product of all argument values                                                 |
| RADIANS ( ***angle*** )                                 | Numerical value | Convert angles (in degrees) to radians                                         |
| RAND()                                            | Numerical value | Random numbers greater than or equal to 0 and less than 1                      |
| ROUND ( ***number, number of digits*** )               | Numerical value | Round the number to the number of digits                                       |
| ROUNDDOWN ( ***number, number of digits*** )           | Numerical value | Truncate the number to the number of digits                                    |
| ROUNDUP ( ***number, number of digits*** )             | Numerical value | Round up the number to the number of digits                                    |
| SIGN ( ***numerical value*** )                          | Numerical value | Positive or negative numbers ( 1 for positive , 0 for 0 , -1 for negative )    |
| SIN ( ***numerical value*** )                           | Numerical value | Numerical sign                                                                 |
| SINH ( ***numerical value*** )                          | Numerical value | Numerical value Hyperbolic sine (hyperbolic sine)                              |
| SQRT ( ***numerical value*** )                          | Numerical value | Positive square root of the number                                             |
| SQUARE ( ***numerical value*** )                        | Numerical value | Number square (square)                                                         |
| SUM ( ***number 1, number 2, ...***)                  | Numerical value | Sum of all argument values                                                     |
| SUMIF ( ***range, search conditions, total range*** ) | Numerical value | Find the sum of the numbers that match the search criteria in the range        |
| SUMSQ ( ***number 1, number 2, ...***)                | Numerical value | Sum of squares of all argument values (sum of squares)                         |
| TAN ( ***numerical value*** )                           | Numerical value | Numerical tangent                                                              |
| TANH ( ***numerical value*** )                          | Numerical value | Numerical hyperbolic tangent (hyperbolic tangent)                              |
| TRUNC ( ***number, number of digits*** )               | Numerical value | Round down the fractional part of theto the number of digits                   |
| XROOT ( ***number, x*** )                              | Numerical value | Returns the value of the xth root of a number .                                |