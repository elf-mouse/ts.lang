## Static Typing

```ts
var burger: string = 'hamburger',     // String
    calories: number = 300,           // Numeric
    tasty: boolean = true;            // Boolean

// Alternatively, you can omit the type declaration:
// var burger = 'hamburger';

// The function expects a string and an integer.
// It doesn't return anything so the type of the function itself is void.

function speak(food: string, energy: number): void {
  console.log("Our " + food + " has " + energy + " calories.");
}

speak(burger, calories);
```

```js
// JavaScript code from the above TS example.

var burger = 'hamburger',
    calories = 300,
    tasty = true;

function speak(food, energy) {
    console.log("Our " + food + " has " + energy + " calories.");
}

speak(burger, calories);
```

Here are some of the most commonly used data types:

- __Number__ – All numeric values are represented by the number type, there aren’t separate definitions for integers, floats or others.
- __String__ – The text type, just like in vanilla JS strings can be surrounded by ‘single quotes’ or “double quotes”.
- __Boolean__ – `true` or `false`, using 0 and 1 will cause a compilation error.
- __Any__ – A variable with this type can have it’s value set to a string, number, or anything else.
- __Arrays__ – Has two possible syntaxes: `my_arr: number[];` or `my_arr: Array<number>`.
- __Void__ – Used on function that don’t return anything.

> To see a list of all of the available types, go to the official TypeScript docs – [here](http://www.typescriptlang.org/docs/handbook/basic-types.html).
