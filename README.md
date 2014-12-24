#  [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-url]][daviddm-image]

> A promises-based wrapper for request


## Install

```sh
$ npm install --save promising-request
```

## Usage

Use everything as you normally would use if it were [request](https://www.npmjs.com/package/request) but every HTTP method returns a promise.

```js
var promisingRequest = require('promising-request');

var promisedLuke = promisingRequest.get('http://swapi.co/api/people/1');

promisedLuke.then(function(res) {
  //fiddle with response
}, function(err) {
  //or handle the errors
});
```


## License

MIT © [Fábio Oliveira](http://about.me/foliveira)


[npm-url]: https://npmjs.org/package/promising-request
[npm-image]: https://badge.fury.io/js/promising-request.svg
[travis-url]: https://travis-ci.org/foliveira/promising-request
[travis-image]: https://travis-ci.org/foliveira/promising-request.svg?branch=master
[daviddm-url]: https://david-dm.org/foliveira/promising-request.svg?theme=shields.io
[daviddm-image]: https://david-dm.org/foliveira/promising-request
