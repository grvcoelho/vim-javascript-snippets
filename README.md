# vim-javascript-snippets
[![Build Status](https://travis-ci.org/grvcoelho/vim-javascript-snippets.svg?branch=master)](https://travis-ci.org/grvcoelho/vim-javascript-snippets)

A collection of Javascript (with ES2015 and Node.js) snippets for Vim heavily based on the work of awesome people like [@zenorocha](https://github.com/zenorocha) and [@msanders](https://github.com/msanders) and powered by [vim-snipmate](https://github.com/garbas/vim-snipmate).

## Install

You need [vim-snipmate](https://github.com/garbas/vim-snipmate) installed. You can then install, using [Plug](https://github.com/junegunn/vim-plug) (or any other vim plugin manager you want):

```
Plug 'grvcoelho/vim-javascript-snippets'
```

## Console

### [cd] console.dir

```javascript
console.dir(${1:obj});
```

### [ce] console.error

```javascript
console.error(${1:obj});
```

### [ci] console.info

```javascript
console.info(${1:obj});
```

### [cl] console.log

```javascript
console.log(${1:obj});
```

### [cw] console.warn

```javascript
console.warn(${1:obj});
```

### [de] debugger

```javascript
debugger;
```

## License
[MIT](https://github.com/grvcoelho/pagarme-node/blob/master/LICENSE) &copy; 2016
