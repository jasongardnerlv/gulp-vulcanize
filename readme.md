# [gulp](http://gulpjs.com)-vulcanize [![Build Status](https://travis-ci.org/sindresorhus/gulp-vulcanize.svg?branch=master)](https://travis-ci.org/sindresorhus/gulp-vulcanize)

> Concatenate a set of Web Components into one file with [Vulcanize](https://github.com/Polymer/vulcanize)

*Issues with the output should be reported on the Vulcanize [issue tracker](https://github.com/Polymer/vulcanize/issues).*


## Install

```bash
$ npm install --save-dev gulp-vulcanize
```


## Usage

```js
var gulp = require('gulp');
var vulcanize = require('gulp-vulcanize');

gulp.task('default', function () {
	gulp.src('src/index.html')
		.pipe(vulcanize({dest: 'dist'}))
		.pipe(gulp.dest('dist'));
});
```


## API

### vulcanize(options)

Same as [grunt-vulcanize](https://github.com/Polymer/grunt-vulcanize#options) plus the below.

#### options.dest

Type: `String`

The destination directory.

Unfortunately needed to get correct relative paths in the output.


## License

[MIT](http://opensource.org/licenses/MIT) © [Sindre Sorhus](http://sindresorhus.com)
