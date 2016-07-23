## Interfaces

```ts
// Here we define our Food interface, its properties, and their types.
interface Food {
    name: string;
    calories: number;
}

// We tell our function to expect an object that fulfills the Food interface.
// This way we know that the properties we need will always be available.
function speak(food: Food): void{
  console.log("Our " + food.name + " has " + food.calories + " calories.");
}

// We define an object that has all of the properties the Food interface expects.
// Notice that types will be inferred automatically.
var ice_cream = {
  name: "ice cream",
  calories: 200
}

speak(ice_cream);
```

> This is a beginners guide so we won’t be going into more detail about interfaces. However, there is a lot more to them than what we’ve mentioned here so we recommend you check out the TypeScript docs – [here](http://www.typescriptlang.org/docs/handbook/interfaces.html).
