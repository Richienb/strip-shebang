# strip-shebang [![Build Status](https://travis-ci.org/sindresorhus/strip-shebang.svg?branch=master)](https://travis-ci.org/sindresorhus/strip-shebang)

> Strip [shebang](https://en.wikipedia.org/wiki/Shebang_(Unix)) *(eg. `#!/bin/sh`)* from a string


## Install

```
$ npm install --save strip-shebang
```


## Usage

```js
const fs = require('fs');
const stripShebang = require('strip-shebang');

const str = fs.readFileSync('bin', 'utf8');
//=> #!/usr/bin/env node
//=> console.log('unicorns');

stripShebang(str);
//=>
//=> console.log('unicorns');
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
