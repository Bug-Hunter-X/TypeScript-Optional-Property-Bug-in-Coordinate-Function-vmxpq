# TypeScript Optional Property Bug

This repository demonstrates a common, yet subtle, bug in TypeScript related to optional properties. The `printCoord` function expects an object with both `x` and `y` properties. However, if you call the function with an object missing either property, the TypeScript compiler won't catch the error and the program may behave unexpectedly at runtime. The solution showcases how to handle optional properties correctly and prevent this runtime error. 

## Bug

The `bug.ts` file contains the buggy code.  The `printCoord` function doesn't explicitly handle cases where `x` or `y` might be missing, leading to a potential runtime error if an incomplete coordinate object is passed.