# Javascript

* Use [ESLint](http://eslint.org/) for linting
* Use [Foo() ESLint config](https://github.com/FooStudio/eslint-config-foo)
* Use [Webpack](https://webpack.github.io/) as the module bundler.
* Javascript Style Guide for ES6 [Airbnb Javascript Style Guide](https://github.com/airbnb/javascript)
* Prefer [ES6 classes](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Classes) over prototypes.
* Avoid having files longer than 100 lines (Excluding comments and line breaks) (Object literals and array declarations in multi-lines count as one).
* Use strict equality checks (`===` and `!==` ) except when comparing against (`null` or `undefined`).
* Prefer [arrow functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) `=>`, over the `function` keyword except when defining classes or methods.
* Prefer method shorthand declaration: `method(){}`        
* Use semicolons at the end of each statement.
* Use `PascalCase` for classes, `lowerCamelCase` for variables and functions, `SCREAMING_SNAKE_CASE` for constants, `_singleLeadingUnderscore` for private variables and functions.
* Prefer [template strings](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals) over string concatenations.     
* Prefer [promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) over callbacks.
* Prefer array functions like `map` and `for of` over `for` loops.
* Use `const` for declaring variables that will never be re-assigned, and `let` otherwise.
* Avoid `var` to declare variables.
* Use a trailing comma after each item in a multi-line array or object literal, including the last item.     
        