# crypto.getRandomValues

[![Greenkeeper badge](https://badges.greenkeeper.io/kumavis/polyfill-crypto.getrandomvalues.svg)](https://greenkeeper.io/)

This is a polyfill for `window.crypto.getRandomValues()`.
In place of `Math.random()` it uses the [Mersenne Twister pseudorandom number generator](https://github.com/boo1ean/mersenne-twister) seeded by `Math.random()`.

### security

WARNING:

Prefer a proper cryptographic entropy source over this module.
If you are out of luck you can use this in a pinch.

### usage

```js
window.crypto = { getRandomValues: require('polyfill-crypto.getrandomvalues') }
```
