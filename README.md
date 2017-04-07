# api documentation for  [pug (v0.1.0)](http://jade-lang.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-pug.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pug) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pug.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pug)
#### A clean, whitespace-sensitive template language for writing HTML

[![NPM](https://nodei.co/npm/pug.png?downloads=true)](https://www.npmjs.com/package/pug)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pug/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pug_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pug/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pug/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pug/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca"
    },
    "bin": {
        "jade": "./bin/jade.js"
    },
    "browser": {
        "fs": false
    },
    "bugs": {
        "url": "https://github.com/jadejs/jade/issues"
    },
    "dependencies": {
        "pug-code-gen": "0.0.0",
        "pug-filters": "1.1.0",
        "pug-lexer": "0.0.0",
        "pug-linker": "0.0.0",
        "pug-loader": "0.0.0",
        "pug-parser": "0.0.0",
        "pug-runtime": "0.0.0",
        "pug-strip-comments": "0.0.1"
    },
    "deprecated": "Please update to the latest version of pug, at time of writing that is pug@2.0.0-alpha6",
    "description": "A clean, whitespace-sensitive template language for writing HTML",
    "devDependencies": {
        "browserify": "*",
        "browserify-middleware": "~4.1.0",
        "code-mirror": "~3.22.0",
        "coveralls": "^2.11.2",
        "doctypes": "^1.0.0",
        "express": "^4.10.4",
        "github-basic": "^5.0.0",
        "highlight-codemirror": "^4.6.1",
        "inconsolata": "0.0.2",
        "istanbul": "*",
        "jade-code-mirror": "~1.0.5",
        "jade-highlighter": "~1.0.5",
        "jquery": "^2.1.4",
        "jstransformer-cdata": "^1.0.0",
        "jstransformer-coffee-script": "^1.0.0",
        "jstransformer-less": "^2.1.0",
        "jstransformer-markdown-it": "^0.2.2",
        "jstransformer-stylus": "^1.0.0",
        "jstransformer-uglify-js": "^1.1.1",
        "jstransformer-verbatim": "^1.0.0",
        "less-file": "0.0.9",
        "linify": "*",
        "lsr": "^1.0.0",
        "markdown-it": "^5.0.1",
        "mocha": "*",
        "pull-request": "^3.0.0",
        "rimraf": "^2.2.8",
        "should": "*",
        "stop": "^3.0.0-rc1",
        "stylus": "*",
        "twbs": "0.0.6",
        "uglify-js": "^2.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "6958bf32ad56378b048f01949b380d470d8b5cc9",
        "tarball": "https://registry.npmjs.org/pug/-/pug-0.1.0.tgz"
    },
    "gitHead": "3ec1aea509172e1c79589487814bd4b0ffce8451",
    "homepage": "http://jade-lang.com",
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "davidglivar",
            "email": "davidglivar@gmail.com"
        },
        {
            "name": "forbeslindesay",
            "email": "forbes@lindesay.co.uk"
        }
    ],
    "name": "pug",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jadejs/jade.git"
    },
    "scripts": {
        "coverage": "istanbul cover node_modules/mocha/bin/_mocha -- -R dot",
        "coveralls": "npm run coverage && cat ./coverage/lcov.info | coveralls",
        "prepublish": "npm prune && linify transform bin",
        "test": "mocha -R spec"
    },
    "version": "0.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pug](#apidoc.module.pug)
1.  [function <span class="apidocSignatureSpan">pug.</span>__express (path, options, fn)](#apidoc.element.pug.__express)
1.  [function <span class="apidocSignatureSpan">pug.</span>compile (str, options)](#apidoc.element.pug.compile)
1.  [function <span class="apidocSignatureSpan">pug.</span>compileClient (str, options)](#apidoc.element.pug.compileClient)
1.  [function <span class="apidocSignatureSpan">pug.</span>compileClientWithDependenciesTracked (str, options)](#apidoc.element.pug.compileClientWithDependenciesTracked)
1.  [function <span class="apidocSignatureSpan">pug.</span>compileFile (path, options)](#apidoc.element.pug.compileFile)
1.  [function <span class="apidocSignatureSpan">pug.</span>compileFileClient (path, options)](#apidoc.element.pug.compileFileClient)
1.  [function <span class="apidocSignatureSpan">pug.</span>render (str, options, fn)](#apidoc.element.pug.render)
1.  [function <span class="apidocSignatureSpan">pug.</span>renderFile (path, options, fn)](#apidoc.element.pug.renderFile)
1.  object <span class="apidocSignatureSpan">pug.</span>cache
1.  object <span class="apidocSignatureSpan">pug.</span>filters
1.  object <span class="apidocSignatureSpan">pug.</span>runtime



# <a name="apidoc.module.pug"></a>[module pug](#apidoc.module.pug)

#### <a name="apidoc.element.pug.__express"></a>[function <span class="apidocSignatureSpan">pug.</span>__express (path, options, fn)](#apidoc.element.pug.__express)
- description and source-code
```javascript
__express = function (path, options, fn) {
  if(options.compileDebug == undefined && process.env.NODE_ENV === 'production') {
    options.compileDebug = false;
  }
  exports.renderFile(path, options, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pug.compile"></a>[function <span class="apidocSignatureSpan">pug.</span>compile (str, options)](#apidoc.element.pug.compile)
- description and source-code
```javascript
compile = function (str, options){
  var options = options || {}

  str = String(str);

  var parsed = compileBody(str, {
    compileDebug: options.compileDebug !== false,
    filename: options.filename,
    basedir: options.basedir,
    pretty: options.pretty,
    doctype: options.doctype,
    inlineRuntimeFunctions: options.inlineRuntimeFunctions,
    globals: options.globals,
    self: options.self,
    includeSources: options.compileDebug === true,
    debug: options.debug,
    templateName: 'template'
  });

  var res = options.inlineRuntimeFunctions
    ? new Function('', parsed.body + ';return template;')()
    : runtimeWrap(parsed.body);

  res.dependencies = parsed.dependencies;

  return res;
}
```
- example usage
```shell
...

For full API, see [jade-lang.com/api](http://jade-lang.com/api/)

'''js
var jade = require('jade');

// compile
var fn = jade.compile('string of jade', options);
var html = fn(locals);

// render
var html = jade.render('string of jade', merge(options, locals));

// renderFile
var html = jade.renderFile('filename.jade', merge(options, locals));
...
```

#### <a name="apidoc.element.pug.compileClient"></a>[function <span class="apidocSignatureSpan">pug.</span>compileClient (str, options)](#apidoc.element.pug.compileClient)
- description and source-code
```javascript
compileClient = function (str, options) {
  return exports.compileClientWithDependenciesTracked(str, options).body;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pug.compileClientWithDependenciesTracked"></a>[function <span class="apidocSignatureSpan">pug.</span>compileClientWithDependenciesTracked (str, options)](#apidoc.element.pug.compileClientWithDependenciesTracked)
- description and source-code
```javascript
compileClientWithDependenciesTracked = function (str, options){
  var options = options || {};

  str = String(str);
  var parsed = compileBody(str, {
    compileDebug: options.compileDebug,
    filename: options.filename,
    basedir: options.basedir,
    pretty: options.pretty,
    doctype: options.doctype,
    inlineRuntimeFunctions: options.inlineRuntimeFunctions !== false,
    globals: options.globals,
    self: options.self,
    includeSources: options.compileDebug,
    debug: options.debug,
    templateName: options.name || 'template'
  });

  return {body: parsed.body, dependencies: parsed.dependencies};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pug.compileFile"></a>[function <span class="apidocSignatureSpan">pug.</span>compileFile (path, options)](#apidoc.element.pug.compileFile)
- description and source-code
```javascript
compileFile = function (path, options) {
  options = options || {};
  options.filename = path;
  return handleTemplateCache(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pug.compileFileClient"></a>[function <span class="apidocSignatureSpan">pug.</span>compileFileClient (path, options)](#apidoc.element.pug.compileFileClient)
- description and source-code
```javascript
compileFileClient = function (path, options){
  var key = path + ':client';
  options = options || {};

  options.filename = path;

  if (options.cache && exports.cache[key]) {
    return exports.cache[key];
  }

  var str = fs.readFileSync(options.filename, 'utf8');
  var out = exports.compileClient(str, options);
  if (options.cache) exports.cache[key] = out;
  return out;
}
```
- example usage
```shell
...



var jade = require('./');
var resolvedJade = require.resolve('./');

function compileTemplate(module, filename) {
var template = jade.compileFileClient(filename, {inlineRuntimeFunctions: false});
var body = "var jade = require('" + resolvedJade + "').runtime;\n\n" +
           "module.exports = " + template + ";";
module._compile(body, filename);
}

if (require.extensions) {
require.extensions['.jade'] = compileTemplate
...
```

#### <a name="apidoc.element.pug.render"></a>[function <span class="apidocSignatureSpan">pug.</span>render (str, options, fn)](#apidoc.element.pug.render)
- description and source-code
```javascript
render = function (str, options, fn){
  // support callback API
  if ('function' == typeof options) {
    fn = options, options = undefined;
  }
  if (typeof fn === 'function') {
    var res
    try {
      res = exports.render(str, options);
    } catch (ex) {
      return fn(ex);
    }
    return fn(null, res);
  }

  options = options || {};

  // cache requires .filename
  if (options.cache && !options.filename) {
    throw new Error('the "filename" option is required for caching');
  }

  return handleTemplateCache(options, str)(options);
}
```
- example usage
```shell
...
var jade = require('jade');

// compile
var fn = jade.compile('string of jade', options);
var html = fn(locals);

// render
var html = jade.render('string of jade', merge(options, locals));

// renderFile
var html = jade.renderFile('filename.jade', merge(options, locals));
'''

### Options
...
```

#### <a name="apidoc.element.pug.renderFile"></a>[function <span class="apidocSignatureSpan">pug.</span>renderFile (path, options, fn)](#apidoc.element.pug.renderFile)
- description and source-code
```javascript
renderFile = function (path, options, fn){
  // support callback API
  if ('function' == typeof options) {
    fn = options, options = undefined;
  }
  if (typeof fn === 'function') {
    var res
    try {
      res = exports.renderFile(path, options);
    } catch (ex) {
      return fn(ex);
    }
    return fn(null, res);
  }

  options = options || {};

  options.filename = path;
  return handleTemplateCache(options)(options);
}
```
- example usage
```shell
...
var fn = jade.compile('string of jade', options);
var html = fn(locals);

// render
var html = jade.render('string of jade', merge(options, locals));

// renderFile
var html = jade.renderFile('filename.jade', merge(options, locals));
'''

### Options

- 'filename'  Used in exceptions, and required when using includes
- 'compileDebug'  When 'false' no debug instrumentation is compiled
- 'pretty'    Add pretty-indentation whitespace to output _(false by default)_
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
