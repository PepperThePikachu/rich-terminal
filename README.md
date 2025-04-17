## Install

```bash
npm install rich-terminal
```

## Info
> Terminal string styling, done simply.

This project relies on Chalk to function, and is at most a wrapper for Chalk.
Please make sure to check it out [here](https://www.npmjs.com/package/chalk). ❤️

## What is this?
This is a project made to simplify string styling, with the goal to make it resemble the functions offered by the [Rich Python Package](https://pypi.org/project/rich/).

## ⚠️ IMPORTANT ⚠️
This project is still in development, and is definitly lacking core features.
Feel free to leave suggestions, beware rich-terminal only supports basic styling at the moment.

## Usage
To get started with this package, import and construct a Console object.
```js
import Console from './index.js'

const console = new Console(); // overrideDefaultLog=true will override console.log() in favor of console.rich()
```

That's it!
We're now ready to start styling our strings. 🔥

```js
console.rich("Hello World!");
```

Just like [Rich](https://pypi.org/project/rich/), rich-terminal offers two ways of styling your output.

### 1. Using tags

```js
console.rich("[bold green]Hello World[/bold green]");
console.rich("[bold green]Hello World[/bold green]");
```

### 2. Using the style property

```js
console.rich({ "Hello", "World" }, { style="bold red" });
```