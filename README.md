BIP39 Mnemonics for Bitcore-Monoeci
=======

[![NPM Package](https://img.shields.io/npm/v/bitcore-mnemonic-monoeci.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-mnemonic-monoeci)
[![Build Status](https://img.shields.io/travis/yoyae/bitcore-mnemonic-monoeci.svg?branch=master&style=flat-square)](https://travis-ci.org/yoyae/bitcore-mnemonic-monoeci)
[![Coverage Status](https://img.shields.io/coveralls/yoyae/bitcore-mnemonic-monoeci.svg?style=flat-square)](https://coveralls.io/r/yoyae/bitcore-mnemonic-monoeci)

A module for [bitcore-monoeci](https://github.com/yoyae/bitcore-monoeci) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-monoeci
bower install bitcore-mnemonic-monoeci
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-monoeci');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/yoyae/bitcore-monoeci/blob/master/CONTRIBUTING.md) on the main bitcore-monoeci repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
