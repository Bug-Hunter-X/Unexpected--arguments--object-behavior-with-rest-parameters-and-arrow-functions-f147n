# Unexpected 'arguments' object behavior with rest parameters and arrow functions

This repository demonstrates an uncommon JavaScript bug related to the `arguments` object when used with rest parameters or arrow functions. The `arguments` object is not available in arrow functions and behaves differently with rest parameters than in traditional functions.

## Bug Description
The `arguments` object in JavaScript is an array-like object containing the arguments passed to a function. However, its behavior is subtle and can lead to unexpected results when used with rest parameters (`...`) or arrow functions (`=>`). In this example, we show that `arguments` is not available in arrow functions. In addition, using rest parameters changes how `arguments` works in normal functions.

## Solution
The solution involves understanding that the `arguments` object is not a true array, and it behaves differently in various function contexts. To achieve similar functionality, use rest parameters directly or spread syntax to collect arguments.