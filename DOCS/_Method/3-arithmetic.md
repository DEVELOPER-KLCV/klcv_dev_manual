---
layout: default
has_children: true

title: Arithmetic Functions
nav_order: 9
permalink: /method/arithmetic
---

# {{ page.title }}

Arithmetic functions are used for general numerical calculations.


| Name        	| Explanation                                                           	|
|-------------	|-----------------------------------------------------------------------	|
| [abs](/method/arithmetic/abs)             | Find the absolute value of a number |
| [and](/method/arithmetic/and)             | Calculate the logical product<br>*<small>Added since Version 5.0.1</small>*<br>*<small>Cannot be used with Mobile & AI version</small>* |
| [int](/method/arithmetic/int)             | Truncate the digits after the decimal point of a floating point number |
| [or](/method/arithmetic/or)               | Find the logical sum<br>*<small>Added since Version 5.0.1</small>*<br>*<small>Cannot be used with Mobile & AI version</small>*|
| [rand](/method/arithmetic/rand)           | Returns a random number in the range 0 to 1 |
| [round](/method/arithmetic/round)         | Round to the specified digit<br>*<small>Added since Version 2.0.0</small>* |
| [rounddown](/method/arithmetic/rounddown) | Truncate at the specified digit<br>*<small>Added since Version 2.0.0</small>*|
| [roundup](/method/arithmetic/roundup)     | Round up to any digit<br>*<small>Added since Version 2.0.0</small>* |
| [roundm](/method/arithmetic/roundm)       | Makes the original value a multiple of the specified value<br>*<small>Added since Version 2.0.0</small>* |
| [sign](/method/arithmetic/sign)           | Determine the sign of a number |
| [xor](/method/arithmetic/xor)             | Find the exclusive OR<br>*<small>Added since Version 5.0.1</small>*<br>*<small>Cannot be used with Mobile & AI version</small>* |


Note that the decimal point operation is a floating point operation internally, so there is a rounding error.
