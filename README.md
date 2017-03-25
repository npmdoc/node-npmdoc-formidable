# api documentation for  [formidable (v1.1.1)](https://github.com/felixge/node-formidable)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-formidable.svg)](https://travis-ci.org/npmdoc/node-npmdoc-formidable)
#### A node.js module for parsing form data, especially file uploads.

[![NPM](https://nodei.co/npm/formidable.png?downloads=true)](https://www.npmjs.com/package/formidable)

[![apidoc](https://npmdoc.github.io/node-npmdoc-formidable/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-formidable_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-formidable/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-formidable/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "bugs": {
        "url": "http://github.com/felixge/node-formidable/issues"
    },
    "dependencies": {},
    "description": "A node.js module for parsing form data, especially file uploads.",
    "devDependencies": {
        "findit": "^0.1.2",
        "gently": "^0.8.0",
        "hashish": "^0.0.4",
        "request": "^2.11.4",
        "urun": "^0.0.6",
        "utest": "^0.0.8"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "96b8886f7c3c3508b932d6bd70c4d3a88f35f1a9",
        "tarball": "https://registry.npmjs.org/formidable/-/formidable-1.1.1.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "7a36a8e932044252fe648c81dbd8cf837d0178d0",
    "homepage": "https://github.com/felixge/node-formidable",
    "license": "MIT",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "felixge",
            "email": "felix@debuggable.com"
        },
        {
            "name": "kornel",
            "email": "pornel@pornel.net"
        },
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        },
        {
            "name": "svnlto",
            "email": "me@svenlito.com"
        },
        {
            "name": "tim-smart",
            "email": "tim@fostle.com"
        },
        {
            "name": "tunnckocore",
            "email": "mameto_100@mail.bg"
        }
    ],
    "name": "formidable",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/felixge/node-formidable.git"
    },
    "scripts": {
        "clean": "rm test/tmp/*",
        "test": "node test/run.js"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module formidable](#apidoc.module.formidable)
1.  [function <span class="apidocSignatureSpan">formidable.</span>IncomingForm (opts)](#apidoc.element.formidable.IncomingForm)
1.  [function <span class="apidocSignatureSpan">formidable.</span>file (properties)](#apidoc.element.formidable.file)
1.  [function <span class="apidocSignatureSpan">formidable.</span>super_ ()](#apidoc.element.formidable.super_)
1.  object <span class="apidocSignatureSpan">formidable.</span>file.prototype
1.  object <span class="apidocSignatureSpan">formidable.</span>incoming_form
1.  object <span class="apidocSignatureSpan">formidable.</span>json_parser
1.  object <span class="apidocSignatureSpan">formidable.</span>multipart_parser
1.  object <span class="apidocSignatureSpan">formidable.</span>octet_parser
1.  object <span class="apidocSignatureSpan">formidable.</span>querystring_parser

#### [module formidable.file](#apidoc.module.formidable.file)
1.  [function <span class="apidocSignatureSpan">formidable.</span>file (properties)](#apidoc.element.formidable.file.file)
1.  [function <span class="apidocSignatureSpan">formidable.file.</span>super_ ()](#apidoc.element.formidable.file.super_)

#### [module formidable.file.prototype](#apidoc.module.formidable.file.prototype)
1.  [function <span class="apidocSignatureSpan">formidable.file.prototype.</span>end (cb)](#apidoc.element.formidable.file.prototype.end)
1.  [function <span class="apidocSignatureSpan">formidable.file.prototype.</span>open ()](#apidoc.element.formidable.file.prototype.open)
1.  [function <span class="apidocSignatureSpan">formidable.file.prototype.</span>toJSON ()](#apidoc.element.formidable.file.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">formidable.file.prototype.</span>write (buffer, cb)](#apidoc.element.formidable.file.prototype.write)

#### [module formidable.incoming_form](#apidoc.module.formidable.incoming_form)
1.  [function <span class="apidocSignatureSpan">formidable.incoming_form.</span>IncomingForm (opts)](#apidoc.element.formidable.incoming_form.IncomingForm)

#### [module formidable.json_parser](#apidoc.module.formidable.json_parser)
1.  [function <span class="apidocSignatureSpan">formidable.json_parser.</span>JSONParser (parent)](#apidoc.element.formidable.json_parser.JSONParser)

#### [module formidable.multipart_parser](#apidoc.module.formidable.multipart_parser)
1.  [function <span class="apidocSignatureSpan">formidable.multipart_parser.</span>MultipartParser ()](#apidoc.element.formidable.multipart_parser.MultipartParser)
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>END
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADERS_ALMOST_DONE
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADER_FIELD
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADER_FIELD_START
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADER_VALUE
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADER_VALUE_ALMOST_DONE
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>HEADER_VALUE_START
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>PARSER_UNINITIALIZED
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>PART_DATA
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>PART_DATA_START
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>PART_END
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>START
1.  number <span class="apidocSignatureSpan">formidable.multipart_parser.</span>START_BOUNDARY

#### [module formidable.octet_parser](#apidoc.module.formidable.octet_parser)
1.  [function <span class="apidocSignatureSpan">formidable.octet_parser.</span>OctetParser (options)](#apidoc.element.formidable.octet_parser.OctetParser)

#### [module formidable.querystring_parser](#apidoc.module.formidable.querystring_parser)
1.  [function <span class="apidocSignatureSpan">formidable.querystring_parser.</span>QuerystringParser (maxKeys)](#apidoc.element.formidable.querystring_parser.QuerystringParser)



# <a name="apidoc.module.formidable"></a>[module formidable](#apidoc.module.formidable)

#### <a name="apidoc.element.formidable.IncomingForm"></a>[function <span class="apidocSignatureSpan">formidable.</span>IncomingForm (opts)](#apidoc.element.formidable.IncomingForm)
- description and source-code
```javascript
function IncomingForm(opts) {
  if (!(this instanceof IncomingForm)) return new IncomingForm(opts);
  EventEmitter.call(this);

  opts=opts||{};

  this.error = null;
  this.ended = false;

  this.maxFields = opts.maxFields || 1000;
  this.maxFieldsSize = opts.maxFieldsSize || 2 * 1024 * 1024;
  this.keepExtensions = opts.keepExtensions || false;
  this.uploadDir = opts.uploadDir || (os.tmpdir && os.tmpdir()) || os.tmpDir();
  this.encoding = opts.encoding || 'utf-8';
  this.headers = null;
  this.type = null;
  this.hash = opts.hash || false;
  this.multiples = opts.multiples || false;

  this.bytesReceived = null;
  this.bytesExpected = null;

  this._parser = null;
  this._flushing = 0;
  this._fieldsSize = 0;
  this.openedFiles = [];

  return this;
}
```
- example usage
```shell
...
var formidable = require('formidable'),
http = require('http'),
util = require('util');

http.createServer(function(req, res) {
  if (req.url == '/upload' && req.method.toLowerCase() == 'post') {
// parse a file upload
var form = new formidable.IncomingForm();

form.parse(req, function(err, fields, files) {
  res.writeHead(200, {'content-type': 'text/plain'});
  res.write('received upload:\n\n');
  res.end(util.inspect({fields: fields, files: files}));
});
...
```

#### <a name="apidoc.element.formidable.file"></a>[function <span class="apidocSignatureSpan">formidable.</span>file (properties)](#apidoc.element.formidable.file)
- description and source-code
```javascript
function File(properties) {
  EventEmitter.call(this);

  this.size = 0;
  this.path = null;
  this.name = null;
  this.type = null;
  this.hash = null;
  this.lastModifiedDate = null;

  this._writeStream = null;

  for (var key in properties) {
    this[key] = properties[key];
  }

  if(typeof this.hash === 'string') {
    this.hash = crypto.createHash(properties.hash);
  } else {
    this.hash = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.formidable.super_"></a>[function <span class="apidocSignatureSpan">formidable.</span>super_ ()](#apidoc.element.formidable.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.formidable.file"></a>[module formidable.file](#apidoc.module.formidable.file)

#### <a name="apidoc.element.formidable.file.file"></a>[function <span class="apidocSignatureSpan">formidable.</span>file (properties)](#apidoc.element.formidable.file.file)
- description and source-code
```javascript
function File(properties) {
  EventEmitter.call(this);

  this.size = 0;
  this.path = null;
  this.name = null;
  this.type = null;
  this.hash = null;
  this.lastModifiedDate = null;

  this._writeStream = null;

  for (var key in properties) {
    this[key] = properties[key];
  }

  if(typeof this.hash === 'string') {
    this.hash = crypto.createHash(properties.hash);
  } else {
    this.hash = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.formidable.file.super_"></a>[function <span class="apidocSignatureSpan">formidable.file.</span>super_ ()](#apidoc.element.formidable.file.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.formidable.file.prototype"></a>[module formidable.file.prototype](#apidoc.module.formidable.file.prototype)

#### <a name="apidoc.element.formidable.file.prototype.end"></a>[function <span class="apidocSignatureSpan">formidable.file.prototype.</span>end (cb)](#apidoc.element.formidable.file.prototype.end)
- description and source-code
```javascript
end = function (cb) {
  var self = this;
  if (self.hash) {
    self.hash = self.hash.digest('hex');
  }
  this._writeStream.end(function() {
    self.emit('end');
    cb();
  });
}
```
- example usage
```shell
...
if (req.url == '/upload' && req.method.toLowerCase() == 'post') {
  // parse a file upload
  var form = new formidable.IncomingForm();

  form.parse(req, function(err, fields, files) {
    res.writeHead(200, {'content-type': 'text/plain'});
    res.write('received upload:\n\n');
    res.end(util.inspect({fields: fields, files: files}));
  });

  return;
}

// show a file upload form
res.writeHead(200, {'content-type': 'text/html'});
...
```

#### <a name="apidoc.element.formidable.file.prototype.open"></a>[function <span class="apidocSignatureSpan">formidable.file.prototype.</span>open ()](#apidoc.element.formidable.file.prototype.open)
- description and source-code
```javascript
open = function () {
  this._writeStream = new fs.WriteStream(this.path);
}
```
- example usage
```shell
...
  name: part.filename,
  type: part.mime,
  hash: self.hash
});

this.emit('fileBegin', part.name, file);

file.open();
this.openedFiles.push(file);

part.on('data', function(buffer) {
  if (buffer.length == 0) {
    return;
  }
  self.pause();
...
```

#### <a name="apidoc.element.formidable.file.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">formidable.file.prototype.</span>toJSON ()](#apidoc.element.formidable.file.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  var json = {
    size: this.size,
    path: this.path,
    name: this.name,
    type: this.type,
    mtime: this.lastModifiedDate,
    length: this.length,
    filename: this.filename,
    mime: this.mime
  };
  if (this.hash && this.hash != "") {
    json.hash = this.hash;
  }
  return json;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.formidable.file.prototype.write"></a>[function <span class="apidocSignatureSpan">formidable.file.prototype.</span>write (buffer, cb)](#apidoc.element.formidable.file.prototype.write)
- description and source-code
```javascript
write = function (buffer, cb) {
  var self = this;
  if (self.hash) {
    self.hash.update(buffer);
  }
  this._writeStream.write(buffer, function() {
    self.lastModifiedDate = new Date();
    self.size += buffer.length;
    self.emit('progress', self.size);
    cb();
  });
}
```
- example usage
```shell
...
http.createServer(function(req, res) {
if (req.url == '/upload' && req.method.toLowerCase() == 'post') {
  // parse a file upload
  var form = new formidable.IncomingForm();

  form.parse(req, function(err, fields, files) {
    res.writeHead(200, {'content-type': 'text/plain'});
    res.write('received upload:\n\n');
    res.end(util.inspect({fields: fields, files: files}));
  });

  return;
}

// show a file upload form
...
```



# <a name="apidoc.module.formidable.incoming_form"></a>[module formidable.incoming_form](#apidoc.module.formidable.incoming_form)

#### <a name="apidoc.element.formidable.incoming_form.IncomingForm"></a>[function <span class="apidocSignatureSpan">formidable.incoming_form.</span>IncomingForm (opts)](#apidoc.element.formidable.incoming_form.IncomingForm)
- description and source-code
```javascript
function IncomingForm(opts) {
  if (!(this instanceof IncomingForm)) return new IncomingForm(opts);
  EventEmitter.call(this);

  opts=opts||{};

  this.error = null;
  this.ended = false;

  this.maxFields = opts.maxFields || 1000;
  this.maxFieldsSize = opts.maxFieldsSize || 2 * 1024 * 1024;
  this.keepExtensions = opts.keepExtensions || false;
  this.uploadDir = opts.uploadDir || (os.tmpdir && os.tmpdir()) || os.tmpDir();
  this.encoding = opts.encoding || 'utf-8';
  this.headers = null;
  this.type = null;
  this.hash = opts.hash || false;
  this.multiples = opts.multiples || false;

  this.bytesReceived = null;
  this.bytesExpected = null;

  this._parser = null;
  this._flushing = 0;
  this._fieldsSize = 0;
  this.openedFiles = [];

  return this;
}
```
- example usage
```shell
...
var formidable = require('formidable'),
http = require('http'),
util = require('util');

http.createServer(function(req, res) {
  if (req.url == '/upload' && req.method.toLowerCase() == 'post') {
// parse a file upload
var form = new formidable.IncomingForm();

form.parse(req, function(err, fields, files) {
  res.writeHead(200, {'content-type': 'text/plain'});
  res.write('received upload:\n\n');
  res.end(util.inspect({fields: fields, files: files}));
});
...
```



# <a name="apidoc.module.formidable.json_parser"></a>[module formidable.json_parser](#apidoc.module.formidable.json_parser)

#### <a name="apidoc.element.formidable.json_parser.JSONParser"></a>[function <span class="apidocSignatureSpan">formidable.json_parser.</span>JSONParser (parent)](#apidoc.element.formidable.json_parser.JSONParser)
- description and source-code
```javascript
function JSONParser(parent) {
  this.parent = parent;
  this.data = new Buffer('');
  this.bytesWritten = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.formidable.multipart_parser"></a>[module formidable.multipart_parser](#apidoc.module.formidable.multipart_parser)

#### <a name="apidoc.element.formidable.multipart_parser.MultipartParser"></a>[function <span class="apidocSignatureSpan">formidable.multipart_parser.</span>MultipartParser ()](#apidoc.element.formidable.multipart_parser.MultipartParser)
- description and source-code
```javascript
function MultipartParser() {
  this.boundary = null;
  this.boundaryChars = null;
  this.lookbehind = null;
  this.state = S.PARSER_UNINITIALIZED;

  this.index = null;
  this.flags = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.formidable.octet_parser"></a>[module formidable.octet_parser](#apidoc.module.formidable.octet_parser)

#### <a name="apidoc.element.formidable.octet_parser.OctetParser"></a>[function <span class="apidocSignatureSpan">formidable.octet_parser.</span>OctetParser (options)](#apidoc.element.formidable.octet_parser.OctetParser)
- description and source-code
```javascript
function OctetParser(options){
	if(!(this instanceof OctetParser)) return new OctetParser(options);
	EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.formidable.querystring_parser"></a>[module formidable.querystring_parser](#apidoc.module.formidable.querystring_parser)

#### <a name="apidoc.element.formidable.querystring_parser.QuerystringParser"></a>[function <span class="apidocSignatureSpan">formidable.querystring_parser.</span>QuerystringParser (maxKeys)](#apidoc.element.formidable.querystring_parser.QuerystringParser)
- description and source-code
```javascript
function QuerystringParser(maxKeys) {
  this.maxKeys = maxKeys;
  this.buffer = '';
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
