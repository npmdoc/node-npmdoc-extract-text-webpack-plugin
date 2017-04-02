# api documentation for  [extract-text-webpack-plugin (v2.1.0)](http://github.com/webpack/extract-text-webpack-plugin)  [![npm package](https://img.shields.io/npm/v/npmdoc-extract-text-webpack-plugin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-extract-text-webpack-plugin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin)
#### Extract text from bundle into a file.

[![NPM](https://nodei.co/npm/extract-text-webpack-plugin.png?downloads=true)](https://www.npmjs.com/package/extract-text-webpack-plugin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-extract-text-webpack-plugin_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screen-capture.npmPackageListing.svg)



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
            "name": "bebraw",
            "email": "bebraw@gmail.com"
        },
        {
            "name": "d3viant0ne",
            "email": "wiens.joshua@gmail.com"
        },
        {
            "name": "ericclemmons",
            "email": "eric@smarterspam.com"
        },
        {
            "name": "jhnns",
            "email": "mail@johannesewald.de"
        },
        {
            "name": "sokra",
            "email": "tobias.koppers@googlemail.com"
        },
        {
            "name": "spacek33z",
            "email": "kees@webduck.nl"
        },
        {
            "name": "thelarkinn",
            "email": "sean.larkin@cuw.edu"
        }
    ],
    "name": "extract-text-webpack-plugin",
    "optionalDependencies": {},
    "peerDependencies": {
        "webpack": "^2.2.0"
    },
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>ExtractedModule (identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>extract ()](#apidoc.element.extract-text-webpack-plugin.extract)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>loader (options)](#apidoc.element.extract-text-webpack-plugin.loader)
1.  object <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>ExtractedModule.prototype

#### [module extract-text-webpack-plugin.ExtractedModule](#apidoc.module.extract-text-webpack-plugin.ExtractedModule)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>ExtractedModule (identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.ExtractedModule)

#### [module extract-text-webpack-plugin.ExtractedModule.prototype](#apidoc.module.extract-text-webpack-plugin.ExtractedModule.prototype)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>addChunk (chunk)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addChunk)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>addPrevModules (prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addPrevModules)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getOrder ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOrder)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getOriginalModule ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOriginalModule)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getPrevModules ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getPrevModules)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>identifier ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.identifier)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>removeChunk (chunk)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.removeChunk)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>rewriteChunkInReasons (oldChunk, newChunks)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.rewriteChunkInReasons)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>setOriginalModule (originalModule)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.setOriginalModule)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>source ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.source)

#### [module extract-text-webpack-plugin.loader](#apidoc.module.extract-text-webpack-plugin.loader)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>loader (source)](#apidoc.element.extract-text-webpack-plugin.loader.loader)
1.  [function <span class="apidocSignatureSpan">extract-text-webpack-plugin.loader.</span>pitch (request)](#apidoc.element.extract-text-webpack-plugin.loader.pitch)



# <a name="apidoc.module.extract-text-webpack-plugin"></a>[module extract-text-webpack-plugin](#apidoc.module.extract-text-webpack-plugin)

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>ExtractedModule (identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule)
- description and source-code
```javascript
function ExtractedModule(identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules) {
	this._identifier = identifier;
	this._originalModule = originalModule;
	this._source = source;
	this._sourceMap = sourceMap;
	this._prevModules = prevModules;
	this.addtitionalInformation = addtitionalInformation;
	this.chunks = [];
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



# <a name="apidoc.module.extract-text-webpack-plugin.ExtractedModule"></a>[module extract-text-webpack-plugin.ExtractedModule](#apidoc.module.extract-text-webpack-plugin.ExtractedModule)

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.ExtractedModule"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>ExtractedModule (identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.ExtractedModule)
- description and source-code
```javascript
function ExtractedModule(identifier, originalModule, source, sourceMap, addtitionalInformation, prevModules) {
	this._identifier = identifier;
	this._originalModule = originalModule;
	this._source = source;
	this._sourceMap = sourceMap;
	this._prevModules = prevModules;
	this.addtitionalInformation = addtitionalInformation;
	this.chunks = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.extract-text-webpack-plugin.ExtractedModule.prototype"></a>[module extract-text-webpack-plugin.ExtractedModule.prototype](#apidoc.module.extract-text-webpack-plugin.ExtractedModule.prototype)

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addChunk"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>addChunk (chunk)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addChunk)
- description and source-code
```javascript
addChunk = function (chunk) {
	var idx = this.chunks.indexOf(chunk);
	if(idx < 0)
		this.chunks.push(chunk);
}
```
- example usage
```shell
...
			if(c.isInitial()) return;
			this.mergeNonInitialChunks(c, chunk, checkedChunks);
		}, this);
	} else if(checkedChunks.indexOf(chunk) < 0) {
		checkedChunks.push(chunk);
		chunk.modules.slice().forEach(function(module) {
			intoChunk.addModule(module);
			module.addChunk(intoChunk);
		});
		chunk.chunks.forEach(function(c) {
			if(c.isInitial()) return;
			this.mergeNonInitialChunks(c, intoChunk, checkedChunks);
		}, this);
	}
};
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addPrevModules"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>addPrevModules (prevModules)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.addPrevModules)
- description and source-code
```javascript
addPrevModules = function (prevModules) {
	prevModules.forEach(function(m) {
		if(this._prevModules.indexOf(m) < 0)
			this._prevModules.push(m);
	}, this);
}
```
- example usage
```shell
...

ExtractTextPluginCompilation.prototype.addModule = function(identifier, originalModule, source, additionalInformation, sourceMap
, prevModules) {
	var m;
	if(!this.modulesByIdentifier[identifier]) {
		m = this.modulesByIdentifier[identifier] = new ExtractedModule(identifier, originalModule, source, sourceMap, additionalInformation
, prevModules);
	} else {
		m = this.modulesByIdentifier[identifier];
		m.addPrevModules(prevModules);
		if(originalModule.index2 < m.getOriginalModule().index2) {
			m.setOriginalModule(originalModule);
		}
	}
	return m;
};
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOrder"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getOrder ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOrder)
- description and source-code
```javascript
getOrder = function () {
	// http://stackoverflow.com/a/14676665/1458162
	return /^@import url/.test(this._source) ? 0 : 1;
}
```
- example usage
```shell
...
function isInvalidOrder(a, b) {
	var bBeforeA = a.getPrevModules().indexOf(b) >= 0;
	var aBeforeB = b.getPrevModules().indexOf(a) >= 0;
	return aBeforeB && bBeforeA;
}

function getOrder(a, b) {
	var aOrder = a.getOrder();
	var bOrder = b.getOrder();
	if(aOrder < bOrder) return -1;
	if(aOrder > bOrder) return 1;
	var aIndex = a.getOriginalModule().index2;
	var bIndex = b.getOriginalModule().index2;
	if(aIndex < bIndex) return -1;
	if(aIndex > bIndex) return 1;
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOriginalModule"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getOriginalModule ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getOriginalModule)
- description and source-code
```javascript
getOriginalModule = function () {
	return this._originalModule;
}
```
- example usage
```shell
...
ExtractTextPluginCompilation.prototype.addModule = function(identifier, originalModule, source, additionalInformation, sourceMap
, prevModules) {
	var m;
	if(!this.modulesByIdentifier[identifier]) {
		m = this.modulesByIdentifier[identifier] = new ExtractedModule(identifier, originalModule, source, sourceMap, additionalInformation
, prevModules);
	} else {
		m = this.modulesByIdentifier[identifier];
		m.addPrevModules(prevModules);
		if(originalModule.index2 < m.getOriginalModule().index2) {
			m.setOriginalModule(originalModule);
		}
	}
	return m;
};

ExtractTextPluginCompilation.prototype.addResultToChunk = function(identifier, result, originalModule, extractedChunk) {
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getPrevModules"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>getPrevModules ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.getPrevModules)
- description and source-code
```javascript
getPrevModules = function () {
	return this._prevModules;
}
```
- example usage
```shell
...
		var moduleSource = module.source();
		source.add(this.applyAdditionalInformation(moduleSource, module.additionalInformation));
	}, this);
	return source;
};

function isInvalidOrder(a, b) {
	var bBeforeA = a.getPrevModules().indexOf(b) >= 0;
	var aBeforeB = b.getPrevModules().indexOf(a) >= 0;
	return aBeforeB && bBeforeA;
}

function getOrder(a, b) {
	var aOrder = a.getOrder();
	var bOrder = b.getOrder();
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.identifier"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>identifier ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.identifier)
- description and source-code
```javascript
identifier = function () {
	return this._identifier;
}
```
- example usage
```shell
...
	var bIndex = b.getOriginalModule().index2;
	if(aIndex < bIndex) return -1;
	if(aIndex > bIndex) return 1;
	var bBeforeA = a.getPrevModules().indexOf(b) >= 0;
	var aBeforeB = b.getPrevModules().indexOf(a) >= 0;
	if(aBeforeB && !bBeforeA) return -1;
	if(!aBeforeB && bBeforeA) return 1;
	var ai = a.identifier();
	var bi = b.identifier();
	if(ai < bi) return -1;
	if(ai > bi) return 1;
	return 0;
}

function ExtractTextPlugin(options) {
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.removeChunk"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>removeChunk (chunk)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.removeChunk)
- description and source-code
```javascript
removeChunk = function (chunk) {
	var idx = this.chunks.indexOf(chunk);
	if(idx >= 0) {
		this.chunks.splice(idx, 1);
		chunk.removeModule(this);
		return true;
	}
	return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.rewriteChunkInReasons"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>rewriteChunkInReasons (oldChunk, newChunks)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.rewriteChunkInReasons)
- description and source-code
```javascript
rewriteChunkInReasons = function (oldChunk, newChunks) { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.setOriginalModule"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>setOriginalModule (originalModule)](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.setOriginalModule)
- description and source-code
```javascript
setOriginalModule = function (originalModule) {
	this._originalModule = originalModule;
}
```
- example usage
```shell
...
	var m;
	if(!this.modulesByIdentifier[identifier]) {
		m = this.modulesByIdentifier[identifier] = new ExtractedModule(identifier, originalModule, source, sourceMap, additionalInformation
, prevModules);
	} else {
		m = this.modulesByIdentifier[identifier];
		m.addPrevModules(prevModules);
		if(originalModule.index2 < m.getOriginalModule().index2) {
			m.setOriginalModule(originalModule);
		}
	}
	return m;
};

ExtractTextPluginCompilation.prototype.addResultToChunk = function(identifier, result, originalModule, extractedChunk) {
	if(!Array.isArray(result)) {
...
```

#### <a name="apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.source"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.ExtractedModule.prototype.</span>source ()](#apidoc.element.extract-text-webpack-plugin.ExtractedModule.prototype.source)
- description and source-code
```javascript
source = function () {
	if(this._sourceMap)
		return new SourceMapSource(this._source, null, this._sourceMap);
	else
		return new RawSource(this._source);
}
```
- example usage
```shell
...
		prevModules.push(module);
	}, this);
};

ExtractTextPlugin.prototype.renderExtractedChunk = function(chunk) {
	var source = new ConcatSource();
	chunk.modules.forEach(function(module) {
		var moduleSource = module.source();
		source.add(this.applyAdditionalInformation(moduleSource, module.additionalInformation));
	}, this);
	return source;
};

function isInvalidOrder(a, b) {
	var bBeforeA = a.getPrevModules().indexOf(b) >= 0;
...
```



# <a name="apidoc.module.extract-text-webpack-plugin.loader"></a>[module extract-text-webpack-plugin.loader](#apidoc.module.extract-text-webpack-plugin.loader)

#### <a name="apidoc.element.extract-text-webpack-plugin.loader.loader"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.</span>loader (source)](#apidoc.element.extract-text-webpack-plugin.loader.loader)
- description and source-code
```javascript
loader = function (source) {
	if(this.cacheable) this.cacheable();
	return source;
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

#### <a name="apidoc.element.extract-text-webpack-plugin.loader.pitch"></a>[function <span class="apidocSignatureSpan">extract-text-webpack-plugin.loader.</span>pitch (request)](#apidoc.element.extract-text-webpack-plugin.loader.pitch)
- description and source-code
```javascript
pitch = function (request) {
	if(this.cacheable) this.cacheable();
	var query = loaderUtils.getOptions(this) || {};
	var loaders = this.loaders.slice(this.loaderIndex + 1);
	this.addDependency(this.resourcePath);
	// We already in child compiler, return empty bundle
	if(this[NS] === undefined) {
		throw new Error(
			'"extract-text-webpack-plugin" loader is used without the corresponding plugin, ' +
			'refer to https://github.com/webpack/extract-text-webpack-plugin for the usage example'
		);
	} else if(this[NS] === false) {
		return "";
	} else if(this[NS](null, query)) {
		if(query.omit) {
			this.loaderIndex += +query.omit + 1;
			request = request.split("!").slice(+query.omit).join("!");
			loaders = loaders.slice(+query.omit);
		}
		var resultSource;
		if(query.remove) {
			resultSource = "// removed by extract-text-webpack-plugin";
		} else {
			resultSource = undefined;
		}

		var childFilename = "extract-text-webpack-plugin-output-filename"; // eslint-disable-line no-path-concat
		var publicPath = typeof query.publicPath === "string" ? query.publicPath : this._compilation.outputOptions.publicPath;
		var outputOptions = {
			filename: childFilename,
			publicPath: publicPath
		};
		var childCompiler = this._compilation.createChildCompiler("extract-text-webpack-plugin", outputOptions);
		childCompiler.apply(new NodeTemplatePlugin(outputOptions));
		childCompiler.apply(new LibraryTemplatePlugin(null, "commonjs2"));
		childCompiler.apply(new NodeTargetPlugin());
		childCompiler.apply(new SingleEntryPlugin(this.context, "!!" + request));
		childCompiler.apply(new LimitChunkCountPlugin({ maxChunks: 1 }));
		var subCache = "subcache " + NS + " " + request; // eslint-disable-line no-path-concat
		childCompiler.plugin("compilation", function(compilation) {
			if(compilation.cache) {
				if(!compilation.cache[subCache])
					compilation.cache[subCache] = {};
				compilation.cache = compilation.cache[subCache];
			}
		});
		// We set loaderContext[NS] = false to indicate we already in
		// a child compiler so we don't spawn another child compilers from there.
		childCompiler.plugin("this-compilation", function(compilation) {
			compilation.plugin("normal-module-loader", function(loaderContext, module) {
				loaderContext[NS] = false;
				if (module.request === request) {
					module.loaders = loaders.map(function(loader) {
						return {
							loader: loader.path,
							options: loader.options
						};
					});
				}
			});
		});

		var source;
		childCompiler.plugin("after-compile", function(compilation, callback) {
			source = compilation.assets[childFilename] && compilation.assets[childFilename].source();

			// Remove all chunk assets
			compilation.chunks.forEach(function(chunk) {
				chunk.files.forEach(function(file) {
					delete compilation.assets[file];
				});
			});

			callback();
		});
		var callback = this.async();
		childCompiler.runAsChild(function(err, entries, compilation) {
			if(err) return callback(err);

			if(compilation.errors.length > 0) {
				return callback(compilation.errors[0]);
			}
			compilation.fileDependencies.forEach(function(dep) {
				this.addDependency(dep);
			}, this);
			compilation.contextDependencies.forEach(function(dep) {
				this.addContextDependency(dep);
			}, this);
			if(!source) {
				return callback(new Error("Didn't get a result from child compiler"));
			}
			try {
				var text = this.exec(source, request);
				if(typeof text === "string")
					text = [[0, text]];
				text.forEach(function(item) {
					var id = item[0];
					compilation.modules.forEach(function(module) {
						if(module.id === id)
							item[0] = module.identifier();
					});
				});
				this[NS](text, query);
				if(text.locals && typeof resultSource !== "undefined") {
					resultSource += "\nmodule.exports = " + JSON.stringify(text.locals) + ";";
				}
			} catch(e) {
				return callback(e);
			}
			if(resultSource)
				callback(null, resultSource);
			else
				callback();
		}.bind(this));
	}
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
