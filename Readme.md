# About [![Build Status](https://travis-ci.org/karpikpl/kattis-js-ecma2016.svg?branch=master)](https://travis-ci.org/karpikpl/kattis-js-ecma2016)
ES2016 wrapper for https://open.kattis.com/ JAVASCRIPT SPIDER MONKEY platform.

## Usage
Run `./start -p [PROBLEM] -w [WORKDIR]` where:
* [PROBLEM] is kattis problem id (from the URL)
* [WORKDIR] is existign working directory - where new folder with the name [PROBLEM] will be created

## Once solution is created
Put your solution inside `solution()` method. Add tests in `test/index.js`.

### Testing
run `npm test` to run mocha unit tests

### Data files
Put data files from kattis into `datafiles` directory in the root folder.
```
index.js
\datafiles
   1.ans
   1.in
```

### Providing input as process params
run `node index.js [input string]`

### Providing input from terminal
run `node index.js i` for interactive mode. Empty line terminates input.

### Submitting to kattis
run `npm start` to transpile code to Firefox 24 - SpiderMonkey version JavaScript-C24.2.0

## Kattis and JavaScript
https://open.kattis.com/help/javascriptspidermonkey
