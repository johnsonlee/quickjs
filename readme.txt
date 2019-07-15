# QuickJS Javascript Engine

## News

- 2019-07-09:
  First public release

## Introduction

QuickJS is a small and embeddable Javascript engine. It supports the ES2019 specification including modules, asynchronous generators and proxies.
It optionally supports mathematical extensions such as big integers (BigInt), big floating point numbers (BigFloat) and operator overloading.

## Main Features:

- Small and easily embeddable: just a few C files, no external dependency, 190 KiB of x86 code for a simple hello world program.
- Fast interpreter with very low startup time: runs the 56000 tests of the ECMAScript Test Suite in about 100 seconds on a single core of a desktop PC. The complete life cycle of a runtime instance completes in less than 300 microseconds.
- Almost complete ES2019 support including modules, asynchronous generators and full Annex B support (legacy web compatibility).
- Passes 100% of the ECMAScript Test Suite.
- Can compile Javascript sources to executables with no external dependency.
- Garbage collection using reference counting (to reduce memory usage and have deterministic behavior) with cycle removal.
- Mathematical extensions: BigInt, BigFloat, operator overloading, bigint mode, math mode.
- Command line interpreter with contextual colorization implemented in Javascript.
- Small built-in standard library with C library wrappers.

## [Benchmark](https://bellard.org/quickjs/bench.html)

## Online Demo

An online demonstration of the QuickJS engine with its mathematical extensions is available at numcalc.com. It was compiled from C to WASM/asm.js with Emscripten.

## Documentation

QuickJS documentation: HTML version, PDF version.
Specification of the JS Bignum Extensions: HTML version, PDF version.

## Sub-projects

QuickJS embeds the following C libraries which can be used in other projects:
- libregexp: small and fast regexp library fully compliant with the Javascript ES 2019 specification.
- libunicode: small unicode library supporting case conversion, unicode normalization, unicode script queries, unicode general category queries and all unicode binary properties.
- libbf: small library implementing arbitrary precision IEEE 754 floating point operations and transcendental functions with exact rounding. It is maintained as a separate project.

## Links

QuickJS Development mailing list

## Licensing

QuickJS is released under the MIT license.
Unless otherwise specified, the QuickJS sources are copyright Fabrice Bellard and Charlie Gordon.

