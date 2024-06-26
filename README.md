# @devtea2028/odio-libero-voluptatem-non <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Set? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isSet = require('@devtea2028/odio-libero-voluptatem-non');
assert(!isSet(function () {}));
assert(!isSet(null));
assert(!isSet(function* () { yield 42; return Infinity; });
assert(!isSet(Symbol('foo')));
assert(!isSet(1n));
assert(!isSet(Object(1n)));

assert(!isSet(new Map()));
assert(!isSet(new WeakSet()));
assert(!isSet(new WeakMap()));

assert(isSet(new Set()));

class MySet extends Set {}
assert(isSet(new MySet()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@devtea2028/odio-libero-voluptatem-non
[npm-version-svg]: https://versionbadg.es/inspect-js/@devtea2028/odio-libero-voluptatem-non.svg
[deps-svg]: https://david-dm.org/inspect-js/@devtea2028/odio-libero-voluptatem-non.svg
[deps-url]: https://david-dm.org/inspect-js/@devtea2028/odio-libero-voluptatem-non
[dev-deps-svg]: https://david-dm.org/inspect-js/@devtea2028/odio-libero-voluptatem-non/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@devtea2028/odio-libero-voluptatem-non#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2028/odio-libero-voluptatem-non.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2028/odio-libero-voluptatem-non.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2028/odio-libero-voluptatem-non.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2028/odio-libero-voluptatem-non
[codecov-image]: https://codecov.io/gh/inspect-js/@devtea2028/odio-libero-voluptatem-non/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@devtea2028/odio-libero-voluptatem-non/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@devtea2028/odio-libero-voluptatem-non
[actions-url]: https://github.com/devtea2028/odio-libero-voluptatem-non/actions
