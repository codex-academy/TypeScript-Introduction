# TypeScript Introduction

## What is TypeScript?

TypeScript is a `Typed superset of JavaScript that transpiles (compiles) into plain JavaScript.` You can read more about it on the [official site](https://www.typescriptlang.org/).

## Install nvm

Node Version Manager aka `nvm` allows you to easily switch between different versions of NodeJS.

Please install it as per the instructions [here](https://github.com/creationix/nvm#install-script)

This will allow you to switch to a newer version on NodeJS easily if you are using advanced JS features in TypeScript that requires ES6 or ES7 features.

## Install TypeScript

You will need TypeScript installed globally.

You can install TypeScript globally using `npm`:

`sudo npm install --g typescript`

You need version `2.2.x` or above. Check your version using the command `tsc -v`

## Using TypeScript

* Create a new folder called `greet-in-typescript`
* Change into it and create a file called `greet.ts`
* Create a function called `greet` which takes a name as a parameter and returns `Hello, <name parameter>`.
* Call the `greet` function and print it's result to the screen.
* Run `tsc greet.ts` this should create a new file called `greet.js`.
* Check the contents of the `greet.js` file - it should look very similar to `greet.ts` except for spacing maybe.
* What happens if you call your greet function with a number parameter?
* Remember to run `tsc greet.ts` again.

At this stage there are no type information in your TypeScript code. Let's fix that.

Change your `greet` function to only take String parameters like this:

```typescript
function greet(name:String){
    //your code here
}
```

Now run `tsc greet.ts` - what happens?

You are getting an error as you can't pass in a number into your `greet` function anymore. The greet function is now `Strongly Typed` and don't allow you to pass in anything, but a string parameter.

### Generating JavaScript automatically

TypeScript can convert `.ts` files into `.js` automatically when they change, by running `tsc` with the `-w` parameter.

Open a new terminal in the same folder (`greet-in-typescript`) and run the `tsc -init` command to create a `tsconfig.json` file. You only have to do this once.

Then run the `tsc -w` command and see what happens if you make changes to your `.ts` files. Try and add a new `.ts` file and to change your `greet.ts`.

## Using TypeScript with Atom

???


## Installed repositories

`npm install --save express`
`npm install --save @types/express`

