# GULP Basics

Gulp is a breeze. Just hack on it for a while and you'll start to see how easy and awesome it is. Here is a starter guide to help you level up.

Since ES6 is a popular now, I'll be showing how to make a Gulpfile the old school way and the ES6 way at the same time.

## NODE First
You can't get yer Gulp on without [Node](https://nodejs.org/en/) installed. Go install that if you haven't done so already.

## Package.json next
With Node installed, you can now create a "package.json" file. NPM stands for "Node Package Manager" and it is included in the Node install you did. Open your Terminal and type `npm init`.

You will be presented with this output first. Read it and press `return` to continue.

```
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg> --save` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
```

Just press `return` through all of the prompts. When you finish it creates a `package.json` file in the directory that you are in. We can forget about this right not, but we will come back to it later.
```
name: (gulp-basics)
version: (1.0.0)
description:
entry point: (index.js)
test command:
git repository:
keywords:
author:
license: (ISC)
About to write to /Users/812studio/Desktop/folders/sites/brownerd/gulp-basics/package.json:

{
  "name": "gulp-basics",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}


Is this ok? (yes)
```

## Global Gulp
Ok, let's install Gulp globally now. Run `npm install gulp -g` in your terminal. If that doesn't take, run `sudo npm install gulp -g`.


## Gulpfile.js
Create a file called `gulpfile.js`. You can do in your editor or from the commandline by typing `touch gulpfile.js`. Your Gulpfile contains all of the "required" modules and "tasks" necessary to run the build processes that you want.

Now let's get Gulp in this project. Run `npm install gulp --save-dev`.

If you look into your `package.json` file, you will notice that it has been updated:

```
"devDependencies": {
  "gulp": "^3.9.0"
}
```
When you install modules using NPM it will create an `node_modules` directory and it will update the `package.json` file to list the dependancies for this project.

## Require/import Gulp
No it is time to get Gulp "into" your gulpfile.

### Old School way
Paste this into your gulpfile `var gulp = require('gulp');`


### ES6 way
Paste this into your gulpfile `import gulp from 'gulp';`

## Updating Node
Sometimes you need to update your version of Node. You can do that my downloading it again: [Node](https://nodejs.org/en/). Or you can do it form the command line : [Upgrade Node.js via NPM](http://davidwalsh.name/upgrade-nodejs)

## Updating Global Packages
Sometimes you need to update the Global packages you installed. Follow these instucitons listed here to do that [Updating global packages](Updating global packages)


## Other Resources
- [Gulp for Beginners](https://css-tricks.com/gulp-for-beginners/)
