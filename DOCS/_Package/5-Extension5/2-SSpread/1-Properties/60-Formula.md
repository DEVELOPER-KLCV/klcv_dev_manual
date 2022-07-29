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
| XROOT ( ***number, x*** )                              | Numerical value | Returns the value of the xth root of a number.                                |

### Logical functions

| Format                                               | Return value  | Description                                                                    | Data editing |
|------------------------------------------------------|---------------|--------------------------------------------------------------------------------|:------------:|
| AND (***Formula 1, Formula 2, ...***)                   | Logical value | Returns TRUE if all argument values are TRUE, FALSE otherwise.               |      Yes     |
| FALSE ()                                             | Logical value | Returns FALSE.                                                                |      No      |
| IF (***logical expression, true value, false value*** ) | Logical value | Returns a true value if the formula is TRUE and a false value if it is FALSE. |      Yes     |
| NOT ( ***logical expression*** )                           | Logical value | Reverse the formula.                                                          |      No      |
| OR (***Formula 1, Formula 2, ...***)                    | Logical value | Returns TRUE if either argument value is TRUE, FALSE otherwise.              |      No      |
| TRUE ()                                              | Logical value | Returns TRUE.                                                                  |      No      |

### Statistical functions

| Format                                              | Return value    | Description                                                                                                                            | 
|-----------------------------------------------------|-----------------|----------------------------------------------------------------------------------------------------------------------------------------|
| AVERAGE (***number 1, number 2, ...***)                | Numerical value | Returns the average of all argument values.                                                                                            |      
| MAX (***number 1, number 2, ...***)                      | Numerical value | Returns the maximum value from all argument values.                                                                                    |      
| MEDIAN (***number 1, number 2, ...***)                   | Numerical value | Returns the median of all argument values.                                                                                             |    
| MIN (***number 1, number 2, ...***)                      | Numerical value | Returns the minimum value of all argument values.                                                                                      |     
| MODE (***number 1, number 2, ...***) | Numerical value | Returns the most frequently occurring value from all argument values.                                                                  |  
| PERMUT (***number, number_chosen***)     | Numerical value | Returns the number of permutations for a given number of objects that can be selected from number objects.                        | 
| RANK (***number, range [, order ]***)                   | Numerical value | Returns the position of the number from the range . If the order is 0, it is in descending order, otherwise it is in ascending order. |         
| STDEV (***number 1, number 2, ...***)                    | Numerical value | Takes all argument values as a sample and returns the standard deviation of the population.                                            |             
| STDEVP (***number 1, number 2, ...***)                   | Numerical value | Considers all argument values as the entire population and returns the standard deviation of the population.                           |            
| VAR (***number 1, number 2, ...***)                      | Numerical value | Takes all argument values as a sample and returns the population variance.                                                             |     
| VARP (***number 1, number 2, ...***)                     | Numerical value | Considers all argument values as the entire population and returns the population variance.                                            |         

### Character functions

| Format                                                                            | Return value    | Description                                                                                                                                                  |
|-----------------------------------------------------------------------------------|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CHAR ( ***number*** )                                                                   | String          | Returns the character corresponding to the number .                                                                                                          |
| CLEAN ( ***string*** )                                                                  | String          | Deletes unprintable characters from the string .                                                                                                             |
| CODE ( ***string*** )                                                                   | Numerical value | Returns the first character of the string as a numeric code.                                                                                                 |
| CONCATENATE ( ***string 1, string 2, ...***)                                          | String          | Combine all argument values into a single string.                                                                                                            |
| EXACT ( ***string 1, string 2*** )                                                     | Logical value   | Returns TRUE if string 1 and string 2 are equal, otherwise FALSE is returned.                                                                                |
| FIND ( ***search string , target [, start position ]***)                                | Numerical value | Searches the search string after thetarget start position and returns the character position.                                                                |
| LEFT ( ***string [, number of characters*** ])                                          | Numerical value | Returns the number of characters from the beginning of the string .                                                                                          |
| LEN ( ***string*** )                                                                    | Numerical value | Returns the number of characters in the string .                                                                                                             |
| LOWER ( ***string*** )                                                                  | String          | Converts a string to lowercase.                                                                                                                              |
| MID ( ***string, start position, number of characters*** )                            | String          | Returns the number of characters fromthe start of the string .                                                                                               |
| PROPER ( ***string*** )                                                                 | String          | Converts the first letter of all English words in the string to uppercase.                                                                                   |
| REPLACE ( ***string, start position, number of characters, replacement string*** )   | String          | Replaces the number of charactersfromthe start of the string with the replacement string .                                                                   |
| REPT ( ***string, number of repetitions*** )                                           | String          | The character string isdisplayed repeatedly as many times as the number of repetitions.                                                                      |
| RIGHT ( ***string [, number of characters ]***)                                         | String          | Returns the number of characters from the right end of the string .                                                                                          |
| SUBSTITUTE ( ***string, search string, replacement string [, replacement target ])*** | String          | Replaces the search string in thewith the replacement string . If you specify a replacement target , only the character string at that position is replaced. |
| TRIM ( ***string*** )                                                                   | String          | Removes extra space from the string .                                                                                                                        |
| UPPER ( ***string*** )                                                                  | String          | Converts a string to uppercase.                                                                                                                              |

### Date / Time functions

| Format                                | Return value    | Description                                                                                                                                                                                          |
|---------------------------------------|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DATE ( ***year, month, day***  )           | Numerical value | Returns consecutive values corresponding to year, month, and day.                                                                                                                                 |
| DAY ( ***continuous value***  )              | Numerical value | Returns the day ( 1 to 31 ) from the date represented by the continuous value.                                                                                                                      |
| HOUR ( ***continuous value***  )             | Numerical value | Returns the time ( 0-23 ) from the time represented by the continuous value.                                                                                                                        |
| MINUTE ( ***continuous value***  )           | Numerical value | Returns the minutes ( 0 to 59 ) from the time represented by the continuous value.                                                                                                                  |
| MONTH ( ***continuous value***  )            | Numerical value | Returns the month ( 1-12 ) fromthe date represented by the continuous value.                                                                                                                        |
| NOW ()                                | Numerical value | Returns a continuous value that represents the current date and time.                                                                                                                                |
| SECOND ( ***continuous value***  )           | Numerical value | Returns seconds ( 0 to 59 ) from the time represented by the continuous value .                                                                                                                       |
| TIME ( ***hours, minutes, seconds***  )    | Numerical value | Returns continuous values corresponding to hours, minutes, and seconds .                                                                                                                           |
| TODAY ()                              | Numerical value | Returns a continuous value that represents the current date.                                                                                                                                         |
| WEEKDAY ( ***continuous value [, type ]*** ) | Numerical value | Returns the day of the week from the date represented by the continuous value . Returns 1 (Sunday) to 7 (Saturday) for type 1, 1 ( Monday) to 7 (Sunday) for 2, and 0 (Monday) to 6 (Sunday) for 3 . |
| YEAR ( ***continuous value*** )             | Numerical value | Returns the year from the date represented by the continuous value.                                                                                                                                 |

### Financial functions

| Format                                                                                                                                | Return value    | Description                                                                                                                                                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DB (***acquisition price, salvage value, useful life, period [, month ]***)                                                             | Numerical value | Use the declining balance method to calculate the depreciation cost of an asset for a particular period.                                                                                             |
| DDB (***acquisition price , salvage value , useful life , period [, rate ]***)                                                             | Numerical value | Use the double declining balance method to calculate the depreciation cost of an asset for a particular period.                                                                                      |
| FV (***interest rate , period , recurring payment amount [, present value [, due date ]]***)                                               | Numerical value | Calculates the future value of the investment, subject to the specified arguments.                                                                                                                   |
| NPER (***interest rate , recurring payment amount , present value [, future value [, due date ]]***)                                       | Numerical value | Calculates the period required for investment (number of payments) with the specified argument as a condition.                                                                                       |
| PMT (***present value , interest rate , total number of payments, number of annual payments***) <br><small>* Specifications are different from Excel</small> | Numerical value | Returns the recurring payment amount for the investment, subject to the specified arguments.                                                                                                         |
| PV (***interest rate , period , recurring payment amount [, future value [, due date ]]***)                                                | Numerical value | Calculates the present value of the investment, subject to the specified arguments.                                                                                                                  |
| SLN (***acquisition price , salvage value , useful life***)                                                                               | Numerical value | Calculate the depreciation cost of an asset per period using the straight-line method.                                                                                                               |
| SYD (***acquisition price , salvage value , useful life , period***)                                                                      | Numerical value | Use the straight-line depreciation method to calculate the depreciation cost of an asset for a particular period.                                                                                    |
| TODAY ()                                                                                                                              | Numerical value | Returns a continuous value that represents the current date.                                                                                                                                         |
| WEEKDAY (***continuous value [, type ]***)                                                                                                 | Numerical value | Returns the day of the week from the date represented by the continuous value . Returns 1 (Sunday) to 7 (Saturday) fortype 1 , 1 ( Monday) to 7 (Sunday) for 2 ,and 0 (Monday) to 6 (Sunday) for 3 . |
| YEAR (***continuous value***)                                                                                                             | Numerical value | Returns the year from the date represented by the continuous value .                                                                                                                                 |

### Information functions

| Format                               | Return value    | Description                                                                                                        |
|--------------------------------------|-----------------|--------------------------------------------------------------------------------------------------------------------|
| COUNT _ _                            | Numerical value | Count the cells of the numeric data in the range.                                                                 |
| COUNTA _ _                           | Numerical value | Count the cells that contain data such as range characters, numbers, and formulas. Unfilled cells are not counted. |
| COUNTIF ( ***range, search condition*** ) | Numerical value | Count the cells that match the search criteria from the range .                                                    |
| ISBLANK ( ***value*** )                    | Logical value   | Returns TRUE if the value is blank, FALSE otherwise.                                                               |
| ISEVEN ( ***value*** )                     | Logical value   | Returns TRUE if the value is even, FALSE otherwise.                                                                |
| ISNONTEXT ( ***value*** )                  | Logical value   | Returns TRUE if the value is non-text, FALSE otherwise.                                                            |
| ISNUMBER _ _                         | Logical value   | Returns TRUE if the value is numeric, FALSE otherwise.                                                             |
| ISODD ( ***value*** )                      | Logical value   | Returns TRUE if the value is odd, FALSE otherwise.                                                                 |
| ISREF ( ***value*** )                      | Logical value   | Returns TRUE if the value is a reference to another cell, FALSE otherwise.                                         |
| ISTEXT ( ***value*** )                     | Logical value   | Returns TRUE if the value is a string, FALSE otherwise.                                                            |

### Other functions

| Format                             | Return value | Description                                   |
|------------------------------------|--------------|-----------------------------------------------|
| URL (***address [, display string ])*** | String       | Create a hyperlink in the exported HTML file. | 