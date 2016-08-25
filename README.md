# Just - Just do one thing.

[![browser support](https://ci.testling.com/justclear/just.png)](https://ci.testling.com/justclear/just)

## Emoji Commit

Commit Type             | Emoji
----------------------- | -------------
Initial Commit          | :tada: `:tada:`
Structure               | :art: `:art:`
Documentation           | :memo: `:memo:`
New Idea                | :bulb: `:bulb:`
New Feature             | :sparkles: `:sparkles:`
Bug                     | :bug: `:bug:`
Version Tag             | :bookmark: `:bookmark:`
Performance             | :racehorse: `:racehorse:`
Tooling                 | :wrench: `:wrench:`
Tests                   | :rotating_light: `:rotating_light:`
Deprecation             | :poop: `:poop:`
Work In Progress (WIP)  | :construction: `:construction:`
Upgrading               | :arrow_up: `:arrow_up:`

Example:

> ":tada: Initial Commit"

## Packages

- <a href="#just-type">just-type</a>
- <a href="#just-camelize">just-camelize</a>

## Usage

<a name="just-type"></a>
### just-type

type checking.

```js
import type from 'just-type';

function hello() {
    console.log('hello type');
}

type(); // undefined
type(undefined); // undefined
type(null); // null
type(''); // string
type('hello'); // string
type(0); // number
type(true); // boolean
type({}); // object
type([]); // array
type(hello); // function
type(/\./); // regexp
```

<a name="just-camelize"></a>
## just-camelize

transform strings to camel case.

```js
import camelize from 'just-camelize';

camelize('_hello_world'); // HelloWorld
camelize('_hello-world'); // HelloWorld
camelize('-hello_world'); // HelloWorld
camelize('-hello-world'); // HelloWorld
```
