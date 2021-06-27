<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# toInt32

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> Convert an unsigned 32-bit integer to a signed 32-bit integer.

<section class="installation">

## Installation

```bash
npm install @stdlib/number-uint32-base-to-int32
```

</section>

<section class="usage">

## Usage

```javascript
var uint32ToInt32 = require( '@stdlib/number-uint32-base-to-int32' );
```

#### uint32ToInt32( x )

Converts an unsigned 32-bit integer to a signed 32-bit integer.

```javascript
var float64ToUint32 = require( '@stdlib/number-float64-base-to-uint32' );

var y = uint32ToInt32( float64ToUint32( 4294967295 ) );
// returns -1

y = uint32ToInt32( float64ToUint32( 3 ) );
// returns 3
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var randu = require( '@stdlib/random-base-randu' );
var MAX_UINT32 = require( '@stdlib/constants-uint32-max' );
var float64ToUint32 = require( '@stdlib/number-float64-base-to-uint32' );
var uint32ToInt32 = require( '@stdlib/number-uint32-base-to-int32' );

var uint32;
var int32;
var i;

for ( i = 0; i < 100; i++ ) {
    // Generate a random unsigned 32-bit integer:
    uint32 = float64ToUint32( randu()*MAX_UINT32 );

    // Convert the unsigned integer to a signed 32-bit integer:
    int32 = uint32ToInt32( uint32 );

    console.log( 'uint32: %d => int32: %d', uint32, int32 );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/number-uint32-base-to-int32.svg
[npm-url]: https://npmjs.org/package/@stdlib/number-uint32-base-to-int32

[test-image]: https://github.com/stdlib-js/number-uint32-base-to-int32/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/number-uint32-base-to-int32/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/number-uint32-base-to-int32/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/number-uint32-base-to-int32?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/number-uint32-base-to-int32.svg
[dependencies-url]: https://david-dm.org/stdlib-js/number-uint32-base-to-int32/main

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/number-uint32-base-to-int32/main/LICENSE

</section>

<!-- /.links -->
