# larg
> A lightweight Node.js argument parser which can be used in various ways.

> [GitHub](https://github.com/PassTheWessel/larg) **|** [NPM](https://npmjs.com/package/larg)

## Installing
```sh
$ yarn add larg # Install w/ Yarn (the superior package manager)
$ npm i larg # Install w/ NPM
```

## Usage
##### Code
```js
const argv = require('larg')(process.argv.slice(2));
console.log(argv);
```
##### Result
```sh
$ node test.js -x 3 -y 4 -ab --beep=boop foo bar
{ _: [ 'foo', 'bar' ],
  x: 3,
  y: 4,
  a: true,
  b: true,
  beep: 'boop' }
```