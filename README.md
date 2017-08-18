## co-eval

Eval with co.
**WARNING: ONLY FOR DEBUG.**

### Install

```bash
$ npm i co-eval -g
```

### Usage

test.js
```javascript
yield blablabla...
```

run:

```bash
$ co test
// or
$ co-eval test
```

equal to:

```
const co = require('co')

co(function* () {
  yield blablabla...
}).catch(console.error)
```