# num-calc

Solve the ECMAScript language large number calculation and floating point number problem.
The underlying method relies on the **BigInt** data type.

## Installation

The num-calc package lives in [npm](https://www.npmjs.com/get-npm). To install the latest stable version, run the following command:

```shell
npm i num-calc
```

Or if you're using [yarn](https://classic.yarnpkg.com/en/docs/install/):

```shell
yarn add num-calc
```
## Usage

[Codepen Demo](https://codepen.io/nickljudy/pen/XWRyQbq)


```js
import { add, sub, multi, devide, calc } from 'num-calc';

add(0.1,0.2) // 0.3
In the same way: calc(0.1,0.2,"+")  //"+" can be replaced by "and"/ "plus"/ "add"

sub(0.3,0.1) //0.2
In the same way: calc(0.3,0.1,"-")  //"-" can be replaced by "minus"/ "sub"/ "subtract"

multi(1.15,100) // 115
In the same way: calc(1.15,100,"*")   //"*" can be replaced by "x"/ "multi"/ "multiply"

devide(9007199254740997,2) //4503599627370498.5
In the same way: calc(1.15,100,"/")   //"/" can be replaced by "divide"

```