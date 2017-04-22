# npmdoc-concat-stream

#### api documentation for  [concat-stream (v1.6.0)](https://github.com/maxogden/concat-stream)  [![npm package](https://img.shields.io/npm/v/npmdoc-concat-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-concat-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-concat-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-concat-stream)

#### writable stream that concatenates strings or binary data and calls a callback with the result

[![NPM](https://nodei.co/npm/concat-stream.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/concat-stream)

- [https://npmdoc.github.io/node-npmdoc-concat-stream/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-concat-stream/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-concat-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Max Ogden"
    },
    "bugs": {
        "url": "http://github.com/maxogden/concat-stream/issues"
    },
    "dependencies": {
        "inherits": "^2.0.3",
        "readable-stream": "^2.2.2",
        "typedarray": "^0.0.6"
    },
    "description": "writable stream that concatenates strings or binary data and calls a callback with the result",
    "devDependencies": {
        "tape": "^4.6.3"
    },
    "directories": {},
    "dist": {
        "shasum": "0aac662fd52be78964d5532f694784e70110acf7",
        "tarball": "https://registry.npmjs.org/concat-stream/-/concat-stream-1.6.0.tgz"
    },
    "engines": [
        "node >= 0.8"
    ],
    "files": [
        "index.js"
    ],
    "gitHead": "e482281642c1e011fc158f5749ef40a71c77a426",
    "homepage": "https://github.com/maxogden/concat-stream",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mafintosh"
        },
        {
            "name": "maxogden"
        }
    ],
    "name": "concat-stream",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/maxogden/concat-stream.git"
    },
    "scripts": {
        "test": "tape test/*.js test/server/*.js"
    },
    "tags": [
        "stream",
        "simple",
        "util",
        "utility"
    ],
    "testling": {
        "files": "test/*.js",
        "browsers": [
            "ie/8..latest",
            "firefox/17..latest",
            "firefox/nightly",
            "chrome/22..latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ]
    },
    "version": "1.6.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
