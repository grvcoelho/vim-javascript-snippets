# vim-javascript-snippets
[![Build Status](https://travis-ci.org/grvcoelho/vim-javascript-snippets.svg?branch=master)](https://travis-ci.org/grvcoelho/vim-javascript-snippets)

A collection of Javascript (with ES2015 and Node.js) snippets for Vim heavily based on the work of awesome people like [@zenorocha](https://github.com/zenorocha), [@msanders](https://github.com/msanders) and [@honza](https://github.com/honza) and powered by [vim-snipmate](https://github.com/garbas/vim-snipmate).

![Demo](https://cloud.githubusercontent.com/assets/7416751/12782176/84ba8efc-ca60-11e5-9be6-8d0221c43a84.gif)

## Install

You need [vim-snipmate](https://github.com/garbas/vim-snipmate) installed. You can then install, using [Plug](https://github.com/junegunn/vim-plug) (or any other vim plugin manager you want):

```
Plug 'grvcoelho/vim-javascript-snippets'
```

## Console

### [cd] console.dir

```javascript
console.dir(${1:obj})
```

### [ce] console.error

```javascript
console.error(${1:obj})
```

### [ci] console.info

```javascript
console.info(${1:obj})
```

### [cl] console.log

```javascript
console.log(${1:obj})
```

### [cw] console.warn

```javascript
console.warn(${1:obj})
```

### [de] debugger

```javascript
debugger
```

## DOM

### [ae] addEventListener

```javascript
${1:document}.addEventListener('${2:event}', ${3:function})
```

### [ac] appendChild
```javascript
${1:document}.appendChild(${2:elem})
```

### [rc] removeChild
```javascript
${1:document}.removeChild(${2:elem})
```

### [cel] createElement
```javascript
${1:document}.createElement(${2:elem})
```

### [cdf] createDocumentFragment
```javascript
${1:document}.createDocumentFragment(${2:elem})
```

### [ca] classList.add
```javascript
${1:document}.classList.add('${2:class}')
```

### [ct] classList.toggle
```javascript
${1:document}.classList.toggle('${2:class}')
```

### [cr] classList.remove
```javascript
${1:document}.classList.remove('${2:class}')
```

### [gi] getElementById
```javascript
${1:document}.getElementById('${2:id}')
```

### [gc] getElementsByClassName
```javascript
${1:document}.getElementsByClassName('${2:class}')
```

### [gt] getElementsByTagName
```javascript
${1:document}.getElementsByTagName('${2:tag}')
```

### [ga] getAttribute
```javascript
${1:document}.getAttribute('${2:attr}')
```

### [sa] setAttribute
```javascript
${1:document}.setAttribute('${2:attr}', ${3:value})
```

### [ra] removeAttribute
```javascript
${1:document}.removeAttribute('${2:attr}')
```

### [ih] innerHTML
```javascript
${1:document}.innerHTML = '${2:elem}'
```

### [tc] textContent
```javascript
${1:document}.textContent = '${2:content}'
```

### [qs] querySelector
```javascript
${1:document}.querySelector('${2:selector}')
```

### [qsa] querySelectorAll
```javascript
${1:document}.querySelectorAll('${2:selector}')
```

## Flow

### [if] if

```javascript
if (${1:condition}) {
	${0}
}
```

### [ife] if else
```javascript
if (${1:condition}) {
	${2}
} else {
	${3}
}
```

### [ifei] if else if

```javascript
if (${1:condition}) {
	${2}
} else if (${3:condition}) {
	${0}
}
```

### [switch] switch

```javascript
switch (${1:condition}) {
	case ${2:when}:
		${0}
}
```

### [tc] try catch

```javascript
try {
	${1}
} catch (${2:err}) {
	${0}
}
```

### [tf] try finally

```javascript
try {
	${1}
} finally {
	${0}
}
```

### [tcf] try catch finally

```javascript
try {
	${1}
} catch (${2:err}) {
	${3}
} finally {
	${0}
}
```

## Function

### [fn] function

```javascript
function ${1:name} (${2}) {
  ${3}
}
```

### [afn] anonymous function

```javascript
function (${1}) {
  ${2}
}
```

### [fgn] generator

```javascript
function* ${1:name} (${2}) {
  ${3}
}
```

### [afgn] anonymous generator

```javascript
function* (${1}) {
  ${2}
}
```

### [afe] arrow function (expression)

```javascript
(${1}) => ${2}
```

### [afb] arrow function (body)
```javascript
(${1}) => {
  ${2}
}
```

## Variables

### [const] const
```
const ${1} = ${0}
```

### [let] let
```javascript
let ${1} = ${0}
```

## JSON

### [jp] json parse

```javascript
JSON.parse(${1:obj})
```

### [js] json stringify

```javascript
JSON.stringify(${1:obj})
```

## Loop

### [for] for
```javascript
for (let i = 0 i < ${1:length} i++) {
	${0}
}
```

### [forin] for in
```javascript
for (${1:prop} in ${2:obj}) {
	if ($2.hasOwnProperty($1)) {
		${0}
	}
}
```

### [forof] for of
```javascript
for (let ${1:elem} of ${2:obj}) {
	${0}
}
```

### [foreach] forEach
```javascript
${1:array}.forEach((${2:item}) => {
	${0}
})
```

### [while] while
```javascript
while (${1:condition}) {
	${0}
}
```

## Class

### [cla] class definition
```javascript
class ${1} {
		${0}
}
```

### [clex] class definition with extends 
```javascript
class ${1} extends ${2} {
		${0}
}
```

## Module

### [imp] import
```javascript
import ${1:module} from '{2:path}'
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License
[MIT](https://github.com/grvcoelho/vim-javascript-snippets/blob/master/LICENSE) &copy; 2016

