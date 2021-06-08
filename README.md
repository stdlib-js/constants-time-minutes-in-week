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

# Minutes in a Week

> Number of minutes in a week.

<section class="installation">

## Installation

```bash
npm install @stdlib/constants-time-minutes-in-week
```

</section>

<section class="usage">

## Usage

```javascript
var MINUTES_IN_WEEK = require( '@stdlib/constants-time-minutes-in-week' );
```

#### MINUTES_IN_WEEK

Number of minutes in a week.

```javascript
var bool = ( MINUTES_IN_WEEK === 10080 );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The value is a generalization and does **not** take into account inaccuracies due to daylight savings conventions, crossing timezones, or other complications with time and dates. 

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var randu = require( '@stdlib/random-base-randu' );
var roundn = require( '@stdlib/math-base-special-roundn' );
var MINUTES_IN_WEEK = require( '@stdlib/constants-time-minutes-in-week' );

var w;
var m;
var i;

function wks2mins( wks ) {
    return wks * MINUTES_IN_WEEK;
}

for ( i = 0; i < 10; i++ ) {
    w = roundn( randu()*20.0, -2 );
    m = wks2mins( w );
    console.log( '%d weeks => %d minutes', w, m );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-time-minutes-in-week/main/LICENSE

</section>

<!-- /.links -->
