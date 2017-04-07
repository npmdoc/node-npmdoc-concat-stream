# api documentation for  [concat-stream (v1.6.0)](https://github.com/maxogden/concat-stream)  [![npm package](https://img.shields.io/npm/v/npmdoc-concat-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-concat-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-concat-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-concat-stream)
#### writable stream that concatenates strings or binary data and calls a callback with the result

[![NPM](https://nodei.co/npm/concat-stream.png?downloads=true)](https://www.npmjs.com/package/concat-stream)

[![apidoc](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-concat-stream_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-concat-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-concat-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Max Ogden",
        "email": "max@maxogden.com"
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
            "name": "mafintosh",
            "email": "mathiasbuus@gmail.com"
        },
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        }
    ],
    "name": "concat-stream",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "1.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module concat-stream](#apidoc.module.concat-stream)
1.  [function <span class="apidocSignatureSpan">concat-stream.</span>super_ (options)](#apidoc.element.concat-stream.super_)
1.  [function <span class="apidocSignatureSpan">concat-stream.</span>super_.WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState)
1.  object <span class="apidocSignatureSpan">concat-stream.</span>super_.WritableState.prototype
1.  object <span class="apidocSignatureSpan">concat-stream.</span>super_.prototype

#### [module concat-stream.super_](#apidoc.module.concat-stream.super_)
1.  [function <span class="apidocSignatureSpan">concat-stream.</span>super_ ()](#apidoc.element.concat-stream.super_.super_)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.</span>WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState)

#### [module concat-stream.super_.WritableState](#apidoc.module.concat-stream.super_.WritableState)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.</span>WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState.WritableState)

#### [module concat-stream.super_.WritableState.prototype](#apidoc.module.concat-stream.super_.WritableState.prototype)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.concat-stream.super_.WritableState.prototype.getBuffer)

#### [module concat-stream.super_.prototype](#apidoc.module.concat-stream.super_.prototype)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>cork ()](#apidoc.element.concat-stream.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>pipe ()](#apidoc.element.concat-stream.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.concat-stream.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>uncork ()](#apidoc.element.concat-stream.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>_writev



# <a name="apidoc.module.concat-stream"></a>[module concat-stream](#apidoc.module.concat-stream)

#### <a name="apidoc.element.concat-stream.super_"></a>[function <span class="apidocSignatureSpan">concat-stream.</span>super_ (options)](#apidoc.element.concat-stream.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.WritableState"></a>[function <span class="apidocSignatureSpan">concat-stream.</span>super_.WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // drain event flag.
  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // when true all writes will be buffered until .uncork() call
  this.corked = 0;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function (er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.bufferedRequest = null;
  this.lastBufferedRequest = null;

  // number of pending user-supplied write callbacks
  // this must be 0 before 'finish' can be emitted
  this.pendingcb = 0;

  // emit prefinish if the only thing we're waiting for is _write cbs
  // This is relevant for synchronous Transform streams
  this.prefinished = false;

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;

  // count buffered requests
  this.bufferedRequestCount = 0;

  // allocate the first CorkedRequest, there is always
  // one allocated and free to use, and we maintain at most two
  this.corkedRequestsFree = new CorkedRequest(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.concat-stream.super_"></a>[module concat-stream.super_](#apidoc.module.concat-stream.super_)

#### <a name="apidoc.element.concat-stream.super_.super_"></a>[function <span class="apidocSignatureSpan">concat-stream.</span>super_ ()](#apidoc.element.concat-stream.super_.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.WritableState"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.</span>WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // drain event flag.
  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // when true all writes will be buffered until .uncork() call
  this.corked = 0;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function (er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.bufferedRequest = null;
  this.lastBufferedRequest = null;

  // number of pending user-supplied write callbacks
  // this must be 0 before 'finish' can be emitted
  this.pendingcb = 0;

  // emit prefinish if the only thing we're waiting for is _write cbs
  // This is relevant for synchronous Transform streams
  this.prefinished = false;

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;

  // count buffered requests
  this.bufferedRequestCount = 0;

  // allocate the first CorkedRequest, there is always
  // one allocated and free to use, and we maintain at most two
  this.corkedRequestsFree = new CorkedRequest(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.concat-stream.super_.WritableState"></a>[module concat-stream.super_.WritableState](#apidoc.module.concat-stream.super_.WritableState)

#### <a name="apidoc.element.concat-stream.super_.WritableState.WritableState"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.</span>WritableState (options, stream)](#apidoc.element.concat-stream.super_.WritableState.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // drain event flag.
  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // when true all writes will be buffered until .uncork() call
  this.corked = 0;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function (er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.bufferedRequest = null;
  this.lastBufferedRequest = null;

  // number of pending user-supplied write callbacks
  // this must be 0 before 'finish' can be emitted
  this.pendingcb = 0;

  // emit prefinish if the only thing we're waiting for is _write cbs
  // This is relevant for synchronous Transform streams
  this.prefinished = false;

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;

  // count buffered requests
  this.bufferedRequestCount = 0;

  // allocate the first CorkedRequest, there is always
  // one allocated and free to use, and we maintain at most two
  this.corkedRequestsFree = new CorkedRequest(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.concat-stream.super_.WritableState.prototype"></a>[module concat-stream.super_.WritableState.prototype](#apidoc.module.concat-stream.super_.WritableState.prototype)

#### <a name="apidoc.element.concat-stream.super_.WritableState.prototype.getBuffer"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.concat-stream.super_.WritableState.prototype.getBuffer)
- description and source-code
```javascript
function getBuffer() {
  var current = this.bufferedRequest;
  var out = [];
  while (current) {
    out.push(current);
    current = current.next;
  }
  return out;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.concat-stream.super_.prototype"></a>[module concat-stream.super_.prototype](#apidoc.module.concat-stream.super_.prototype)

#### <a name="apidoc.element.concat-stream.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>cork ()](#apidoc.element.concat-stream.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...

#### Arrays

'''js
var write = concat(function(data) {})
write.write([1,2,3])
write.write([4,5,6])
write.end()
// data will be [1,2,3,4,5,6] in the above callback
'''

#### Uint8Arrays

'''js
var write = concat(function(data) {})
...
```

#### <a name="apidoc.element.concat-stream.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>pipe ()](#apidoc.element.concat-stream.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.emit('error', new Error('Cannot pipe, not readable'));
}
```
- example usage
```shell
...
var fs = require('fs')
var concat = require('concat-stream')

var readStream = fs.createReadStream('cat.png')
var concatStream = concat(gotPicture)

readStream.on('error', handleError)
readStream.pipe(concatStream)

function gotPicture(imageBuffer) {
// imageBuffer is all of 'cat.png' as a node.js Buffer
}

function handleError(err) {
// handle your error appropriately here, e.g.:
...
```

#### <a name="apidoc.element.concat-stream.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.concat-stream.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>uncork ()](#apidoc.element.concat-stream.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.concat-stream.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">concat-stream.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.concat-stream.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...

'''

#### Arrays

'''js
var write = concat(function(data) {})
write.write([1,2,3])
write.write([4,5,6])
write.end()
// data will be [1,2,3,4,5,6] in the above callback
'''

#### Uint8Arrays
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
