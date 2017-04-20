# npmtest-azure-storage

#### basic test coverage for  [azure-storage (v2.1.0)](http://github.com/Azure/azure-storage-node)  [![npm package](https://img.shields.io/npm/v/npmtest-azure-storage.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-azure-storage) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-azure-storage.svg)](https://travis-ci.org/npmtest/node-npmtest-azure-storage)

#### Microsoft Azure Storage Client Library for Node.js

[![NPM](https://nodei.co/npm/azure-storage.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/azure-storage)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-azure-storage/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-azure-storage/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-azure-storage/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-azure-storage/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-azure-storage/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-azure-storage/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-azure-storage/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-azure-storage/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-azure-storage/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-azure-storage/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-azure-storage/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-azure-storage/build/test-report.html](https://npmtest.github.io/node-npmtest-azure-storage/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-azure-storage/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-azure-storage/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-azure-storage/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-azure-storage/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-azure-storage/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-azure-storage/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-azure-storage/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-azure-storage/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "azure-storage",
    "author": "Microsoft Corporation",
    "version": "2.1.0",
    "description": "Microsoft Azure Storage Client Library for Node.js",
    "typings": "typings/azure-storage/azure-storage.d.ts",
    "tags": [
        "azure",
        "storage",
        "sdk"
    ],
    "keywords": [
        "node",
        "azure",
        "storage"
    ],
    "main": "./lib/azure-storage.js",
    "engines": {
        "node": ">= 0.8.26"
    },
    "license": "Apache-2.0",
    "dependencies": {
        "browserify-mime": "~1.2.9",
        "extend": "~1.2.1",
        "json-edm-parser": "0.1.2",
        "md5.js": "1.3.4",
        "node-uuid": "~1.4.0",
        "readable-stream": "~2.0.0",
        "request": "~2.74.0",
        "underscore": "~1.4.4",
        "validator": "~3.22.2",
        "xml2js": "0.2.7",
        "xmlbuilder": "0.4.3"
    },
    "devDependencies": {
        "browserify": "^13.3.0",
        "browserify-fs": "^1.0.0",
        "batchflow": "0.4.0",
        "coveralls": "^2.11.4",
        "factor-bundle": "^2.5.0",
        "grunt": "~0.4.2",
        "grunt-contrib-jshint": "~0.11.0",
        "grunt-devserver": "^0.6.0",
        "grunt-jsdoc": "~2.1.0",
        "grunt-mocha": "^0.4.12",
        "grunt-mocha-test": "^0.12.7",
        "grunt-nsp": "^2.3.1",
        "ink-docstrap": "^1.3.0",
        "istanbul": "^0.3.22",
        "jshint": ">= 2.1.4",
        "mocha": ">= 1.18.0",
        "mocha-lcov-reporter": "^1.0.0",
        "nock": "0.16",
        "nsp": "^2.2.0",
        "should": "1.2.x"
    },
    "browser": {
        "fs": "browserify-fs"
    },
    "homepage": "http://github.com/Azure/azure-storage-node",
    "repository": {
        "type": "git",
        "url": "git@github.com:Azure/azure-storage-node.git"
    },
    "bugs": {
        "url": "http://github.com/Azure/azure-storage-node/issues"
    },
    "scripts": {
        "check": "jshint lib && nsp check",
        "test": "jshint lib && nsp check && mocha --no-timeouts --recursive test",
        "cover": "istanbul cover ./node_modules/mocha/bin/_mocha -- -R spec -u bdd --no-timeouts --recursive test",
        "coveralls": "npm run cover && cat ./coverage/lcov.info | node ./node_modules/coveralls/bin/coveralls.js",
        "genjs": "node ./browser/bundle.js"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
