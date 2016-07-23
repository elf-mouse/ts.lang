## Compiling to JavaScript

- In the terminal using the previously mentioned command line tool `tsc`.
- Directly in Visual Studio or some of the other IDEs and text editors.
- Using automated task runners such as [gulp](http://gulpjs.com/).

```sh
tsc main.ts
```

```sh
# Will result in separate .js files: main.js worker.js.
tsc main.ts worker.ts

# Compiles all .ts files in the current folder. Does NOT work recursively.
tsc *.ts
```

```sh
# Initializes a watcher process that will keep main.js up to date.
tsc main.ts --watch
```

> More advanced TypeScript users can also create a _tsconfig.json_ file, consisting of various build settings. A configuration file is very handy when working on large projects with lots of .ts files since it somewhat automates the process. You can read more about _tsconfig.json_ in the TypeScript docs [here](http://www.typescriptlang.org/docs/handbook/tsconfig-json.html)
