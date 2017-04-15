# api documentation for  [extract-text-webpack-plugin (v2.1.0)](http://github.com/webpack/extract-text-webpack-plugin)  [![npm package](https://img.shields.io/npm/v/npmdoc-extract-text-webpack-plugin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-extract-text-webpack-plugin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin)
#### Extract text from bundle into a file.

[![NPM](https://nodei.co/npm/extract-text-webpack-plugin.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/extract-text-webpack-plugin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tobias Koppers @sokra"
    },
    "bugs": {
        "url": "https://github.com/webpack/extract-text-webpack-plugin/issues"
    },
    "dependencies": {
        "ajv": "^4.11.2",
        "async": "^2.1.2",
        "loader-utils": "^1.0.2",
        "webpack-sources": "^0.1.0"
    },
    "description": "Extract text from bundle into a file.",
    "devDependencies": {
        "codecov.io": "^0.1.2",
        "coveralls": "^2.11.2",
        "css-loader": "^0.26.1",
        "file-loader": "^0.9.0",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "mocha-lcov-reporter": "1.2.0",
        "raw-loader": "^0.5.1",
        "should": "^11.1.2",
        "standard-version": "^4.0.0",
        "style-loader": "^0.13.0",
        "webpack": "^2.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "69315b885f876dbf96d3819f6a9f1cca7aebf159",
        "tarball": "https://registry.npmjs.org/extract-text-webpack-plugin/-/extract-text-webpack-plugin-2.1.0.tgz"
    },
    "engines": {
        "node": ">=4.3.0 < 5.0.0 || >= 5.10"
    },
    "gitHead": "75cb09eed13d15cec8f974b1210920a7f249f8e2",
    "homepage": "http://github.com/webpack/extract-text-webpack-plugin",
    "license": "MIT",
    "maintainers": [
        {
            "name": "bebraw"
        },
        {
            "name": "d3viant0ne"
        },
        {
            "name": "ericclemmons"
        },
        {
            "name": "jhnns"
        },
        {
            "name": "sokra"
        },
        {
            "name": "spacek33z"
        },
        {
            "name": "thelarkinn"
        }
    ],
    "name": "extract-text-webpack-plugin",
    "optionalDependencies": {},
    "peerDependencies": {
        "webpack": "^2.2.0"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/webpack/extract-text-webpack-plugin.git"
    },
    "scripts": {
        "build:example": "(cd example && webpack)",
        "cover": "istanbul cover _mocha",
        "release": "standard-version",
        "test": "mocha",
        "travis": "npm run cover -- --report lcovonly"
    },
    "version": "2.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module extract-text-webpack-plugin](#apidoc.module.extract-text-webpack-plugin)
1.  [function <span class="apidocSignatureSpan"></span>extract-text-webpack-plugin (options)](#apidoc.element.extract-text-webpack-plugin.extract-text-webpack-plugin)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>extract ()](#apidoc.element.extract-text-webpack-plugin.extract)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>loader (options)](#apidoc.element.extract-text-webpack-plugin.loader)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>toString ()](#apidoc.element.extract-text-webpack-plugin.toString)



# <a name="apidoc.module.extract-text-webpack-plugin"></a>[module extract-text-webpack-plugin](#apidoc.module.extract-text-webpack-plugin)

#### <a name="apidoc.element.extract-text-webpack-plugin.extract-text-webpack-plugin"></a>[function <span class="apidocSignatureSpan"></span>extract-text-webpack-plugin (options)](#apidoc.element.extract-text-webpack-plugin.extract-text-webpack-plugin)
- description and source-code
```javascript
function ExtractTextPlugin(options) {
	if(arguments.length > 1) {
		throw new Error("Breaking change: ExtractTextPlugin now only takes a single argument. Either an options " +
						"object *or* the name of the result file.\n" +
						"Example: if your old code looked like this:\n" +
						"    new ExtractTextPlugin('css/[name].css', { disable: false, allChunks: true })\n\n" +
						"You would change it to:\n" +
						"    new ExtractTextPlugin({ filename: 'css/[name].css', disable: false, allChunks: true })\n\n" +
						"The available options are:\n" +
						"    filename: string\n" +
						"    allChunks: boolean\n" +
						"    disable: boolean\n");
	}
	if(isString(options)) {
		options = { filename: options };
	} else {
		schemaTester(pluginSchema, options);
	}
	this.filename = options.filename;
	this.id = options.id != null ? options.id : ++nextId;
	this.options = {};
	mergeOptions(this.options, options);
	delete this.options.filename;
	delete this.options.id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.extract-text-webpack-plugin.extract"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>extract ()](#apidoc.element.extract-text-webpack-plugin.extract)
- description and source-code
```javascript
extract = function () { [native code] }
```
- example usage
```shell
...
const ExtractTextPlugin = require("extract-text-webpack-plugin");

module.exports = {
module: {
  rules: [
    {
      test: /\.css$/,
      use: ExtractTextPlugin.extract({
        fallback: "style-loader",
        use: "css-loader"
      })
    }
  ]
},
plugins: [
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.loader"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>loader (options)](#apidoc.element.extract-text-webpack-plugin.loader)
- description and source-code
```javascript
loader = function (options) {
	return { loader: require.resolve("./loader"), options: options };
}
```
- example usage
```shell
...
			"}"
		);
	}
	return source;
};

ExtractTextPlugin.prototype.loader = function(options) {
	return ExtractTextPlugin.loader(mergeOptions({id: this.id}, options));
};

ExtractTextPlugin.prototype.extract = function(options) {
	if(arguments.length > 1) {
		throw new Error("Breaking change: extract now only takes a single argument. Either an options " +
						"object *or* the loader(s).\n" +
						"Example: if your old code looked like this:\n" +
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.toString"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>toString ()](#apidoc.element.extract-text-webpack-plugin.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
