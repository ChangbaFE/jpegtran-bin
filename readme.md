# jpegtran-changba [![Build Status](https://travis-ci.org/ChangbaFE/jpegtran-bin.svg?branch=master)](https://travis-ci.org/ChangbaFE/jpegtran-bin)

> [libjpeg-turbo](http://libjpeg-turbo.virtualgl.org/) is a derivative of libjpeg that uses SIMD instructions (MMX, SSE2, NEON) to accelerate baseline JPEG compression and decompression on x86, x86-64, and ARM systems. On such systems, libjpeg-turbo is generally 2-4x as fast as the unmodified version of libjpeg, all else being equal.

You probably want [`imagemin-jpegtran`](https://github.com/imagemin/imagemin-jpegtran) instead.


## Install

```
$ npm install --save jpegtran-changba
```


## Usage

```js
const {execFile} = require('child_process');
const jpegtran = require('jpegtran-changba');

execFile(jpegtran, ['-outfile', 'output.jpg', 'input.jpg'], error => {
	console.log('Image minified!');
});
```


## CLI

```
$ npm install --global jpegtran-changba
```

```
$ jpegtran --help
```


## License

MIT © [Imagemin](https://github.com/imagemin)
