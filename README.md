# numeral-calc

Solve the ECMAScript language **large number calculation** and **floating point number** problem.

Supports scientific numeration calculations.


[![Build Status](https://travis-ci.com/NickLJudy/numeral-calc.svg?branch=main)](https://travis-ci.com/NickLJudy/numeral-calc)
[![Coverage Status](https://coveralls.io/repos/github/NickLJudy/numeral-calc/badge.svg)](https://coveralls.io/github/NickLJudy/numeral-calc)
[![Version](https://img.shields.io/npm/v/numeral-calc.svg?maxAge=300&label=version&colorB=007ec6&maxAge=300)](./package.json)
[![npm bundle size](https://img.shields.io/bundlephobia/minzip/numeral-calc)](https://bundlephobia.com/package/numeral-calc)
![dependencies-logo](https://status.david-dm.org/gh/NickLJudy/numeral-calc.svg)
![last-commit-date-logo](https://img.shields.io/github/last-commit/NickLJudy/numeral-calc)
## Installation

The numeral-calc package lives in [npm](https://www.npmjs.com/get-npm). To install the latest stable version, run the following command:

```shell
npm i numeral-calc
```

Or if you're using [yarn](https://classic.yarnpkg.com/en/docs/install/):

```shell
yarn add numeral-calc
```
## Usage

[Codepen Demo](https://codepen.io/nickljudy/pen/XWRyQbq)


```js
import { add, sub, multi, divide, calc } from 'numeral-calc';

add(0.1,0.2) // "0.3"
In the same way: calc(0.1,0.2,"+")  //  "+" can be replaced by "and" or "plus" or "add"

add(0.1,0.2,1) // "1.3"

sub(0.3,0.1) // "0.2"
In the same way: calc(0.3,0.1,"-")  //  "-" can be replaced by "minus" or "sub" or "subtract"
/* Support for custom scientific notation. */
sub(1.02e1,1.3e-4)  //  "10.19987"

multi(1.15,100) // "115"

multi(1.15,100,2) // "230"
In the same way: calc(1.15,100,"*")   //  "*" can be replaced by "x" or "multi" or "multiply"

divide(9007199254740997,2) // "4503599627370498.5"
In the same way: calc(9007199254740997,2,"/")   //  "/" can be replaced by "divide"

```

## Objective
Use the simplest method to solve the most fundamental problem.
* No new types are generated.
* Floating-point and large numbers are handled together using numeral-calc.

The underlying method relies on the **BigInt** data type.

Addition and multiplication can take multiple arguments.


## Notice

There seems to be no such business scenario. 
* The divisor cannot exceed the safe range of the JS language.
* Scientific notation exponentials cannot exceed the safe limits of the JS language.