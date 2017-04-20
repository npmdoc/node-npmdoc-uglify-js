# npmdoc-uglify-js

#### api documentation for  [uglify-js (v2.8.22)](http://lisperator.net/uglifyjs)  [![npm package](https://img.shields.io/npm/v/npmdoc-uglify-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-uglify-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-uglify-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-uglify-js)

#### JavaScript parser, mangler/compressor and beautifier toolkit

[![NPM](https://nodei.co/npm/uglify-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/uglify-js)

- [https://npmdoc.github.io/node-npmdoc-uglify-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-uglify-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-uglify-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-uglify-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-uglify-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-uglify-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mihai Bazon",
        "url": "http://lisperator.net/"
    },
    "bin": {
        "uglifyjs": "bin/uglifyjs"
    },
    "browserify": {
        "transform": [
            "uglify-to-browserify"
        ]
    },
    "bugs": {
        "url": "https://github.com/mishoo/UglifyJS2/issues"
    },
    "dependencies": {
        "source-map": "~0.5.1",
        "uglify-to-browserify": "~1.0.0",
        "yargs": "~3.10.0"
    },
    "description": "JavaScript parser, mangler/compressor and beautifier toolkit",
    "devDependencies": {
        "acorn": "~0.6.0",
        "escodegen": "~1.3.3",
        "esfuzz": "~0.3.1",
        "estraverse": "~1.5.1",
        "mocha": "~2.3.4"
    },
    "directories": {},
    "dist": {
        "shasum": "d54934778a8da14903fa29a326fb24c0ab51a1a0",
        "tarball": "https://registry.npmjs.org/uglify-js/-/uglify-js-2.8.22.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "files": [
        "bin",
        "lib",
        "tools",
        "LICENSE"
    ],
    "gitHead": "04b89645058d85b8b67bb94fb9e39252160a0959",
    "homepage": "http://lisperator.net/uglifyjs",
    "keywords": [
        "uglify",
        "uglify-js",
        "minify",
        "minifier"
    ],
    "license": "BSD-2-Clause",
    "main": "tools/node.js",
    "maintainers": [
        {
            "name": "alexlamsl"
        },
        {
            "name": "mishoo"
        },
        {
            "name": "rvanvelzen1"
        }
    ],
    "name": "uglify-js",
    "optionalDependencies": {
        "uglify-to-browserify": "~1.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mishoo/UglifyJS2.git"
    },
    "scripts": {
        "test": "node test/run-tests.js"
    },
    "version": "2.8.22"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
