# npmdoc-extract-text-webpack-plugin

#### api documentation for  [extract-text-webpack-plugin (v2.1.0)](http://github.com/webpack/extract-text-webpack-plugin)  [![npm package](https://img.shields.io/npm/v/npmdoc-extract-text-webpack-plugin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-extract-text-webpack-plugin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-extract-text-webpack-plugin)

#### Extract text from bundle into a file.

[![NPM](https://nodei.co/npm/extract-text-webpack-plugin.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/extract-text-webpack-plugin)

- [https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-extract-text-webpack-plugin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "extract-text-webpack-plugin",
    "version": "2.1.0",
    "author": "Tobias Koppers @sokra",
    "description": "Extract text from bundle into a file.",
    "engines": {
        "node": ">=4.3.0 < 5.0.0 || >= 5.10"
    },
    "peerDependencies": {
        "webpack": "^2.2.0"
    },
    "dependencies": {
        "ajv": "^4.11.2",
        "async": "^2.1.2",
        "loader-utils": "^1.0.2",
        "webpack-sources": "^0.1.0"
    },
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
    "homepage": "http://github.com/webpack/extract-text-webpack-plugin",
    "repository": {
        "type": "git",
        "url": "http://github.com/webpack/extract-text-webpack-plugin.git"
    },
    "license": "MIT",
    "scripts": {
        "test": "mocha",
        "travis": "npm run cover -- --report lcovonly",
        "cover": "istanbul cover _mocha",
        "release": "standard-version",
        "build:example": "(cd example && webpack)"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
