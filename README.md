# arraybuffer-equal

Determines if two array buffers contain the exact same content.

## Installation

`npm install --save arraybuffer-equal`

## Usage

```js
var isEqual = require('arraybuffer-equal');

var buf1 = new Uint8Array([0x50, 0x0a]).buffer;
var buf2 = new Uint8Array([0x50, 0x0a]).buffer;
var buf3 = new Uint8Array([0x50, 0x0b]).buffer;
var buf4 = new Uint8Array([0x50, 0x0b, 0x15]).buffer;

assert(isEqual(buf1, buf1));
assert(isEqual(buf1, buf2));
assert(!isEqual(buf1, buf3));
assert(!isEqual(buf1, buf4));
```

## License
(c) 2015 Will Binns-Smith. Licensed MIT.
