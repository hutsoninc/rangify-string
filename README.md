# rangify-string

[![Build Status](https://travis-ci.com/hutsoninc/rangify-string.svg?branch=master)](https://travis-ci.com/hutsoninc/rangify-string) [![Current npm package version](https://img.shields.io/npm/v/rangify-string.svg)](https://www.npmjs.com/package/rangify-string) 

Create an array from a string of integer ranges.

## Installation

`npm install --save rangify-string`

## Usage

```js
const rangify = require('rangify-string');

rangify('1-3,5,9-10');
//=> [1, 2, 3, 5, 9, 10]

rangify('11,15-20');
//=> [11, 15, 16, 17, 18, 19, 20]

rangify('5-7,3-6', {
    sort: false,
    filter: false
})
//=> [5, 6, 7, 3, 4, 5, 6]
```

## Options

Property | Description | Default
--- | --- | ---
sort | Sort the output array | `true`
filter | Filter duplicates from output array | `true`

## Authors

* **Austin Gordon** - *Development* - [GitHub](https://github.com/AustinLeeGordon)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details