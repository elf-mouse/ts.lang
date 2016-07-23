## Modules

__exporter.ts__

```ts
var sayHi = function(): void {
    console.log("Hello!");
}

export = sayHi;
```

__importer.ts__

```ts
import sayHi = require('./exporter');
sayHi();
```

---

```sh
tsc --module amd *.ts
```

> Modules are quite complex and are out of the scope of this tutorial. If you want to continue reading about them head out to the TS docs – [here](http://www.typescriptlang.org/docs/handbook/modules.html).
