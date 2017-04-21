# npmdoc-marsdb

#### api documentation for  [marsdb (v0.6.11)](https://github.com/c58/marsdb)  [![npm package](https://img.shields.io/npm/v/npmdoc-marsdb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-marsdb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-marsdb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-marsdb)

#### MarsDB is a lightweight client-side MongoDB-like database, Promise based, written in ES6

[![NPM](https://nodei.co/npm/marsdb.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/marsdb)

- [https://npmdoc.github.io/node-npmdoc-marsdb/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-marsdb/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-marsdb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-marsdb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-marsdb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-marsdb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "marsdb",
    "version": "0.6.11",
    "author": {
        "name": "Artem Artemev"
    },
    "contributors": [
        "Artem Artemev"
    ],
    "description": "MarsDB is a lightweight client-side MongoDB-like database, Promise based, written in ES6",
    "keywords": [
        "database",
        "datastore",
        "embedded",
        "levelup",
        "mongoose",
        "linvodb3",
        "nedb"
    ],
    "homepage": "https://github.com/c58/marsdb",
    "repository": {
        "type": "git",
        "url": "git@github.com:c58/marsdb.git"
    },
    "dependencies": {
        "check-types": "^6.0.0",
        "double-ended-queue": "^0.9.7",
        "eventemitter3": "1.1.1",
        "fast.js": "^0.1.1",
        "geojson-utils": "^1.1.0",
        "invariant": "^2.2.0"
    },
    "devDependencies": {
        "core-js": "^2.0.1",
        "lodash": "3.10.x",
        "babel-cli": "^6.3.17",
        "babel-eslint": "^5.0.0-beta6",
        "babel-preset-es2015": "^6.3.13",
        "babel-preset-stage-0": "^6.3.13",
        "babel-register": "^6.3.13",
        "babelify": "^7.2.0",
        "brfs": "^1.4.1",
        "browserify": "^13.0.0",
        "bulk-require": "^0.2.1",
        "bulkify": "^1.1.1",
        "chai": "^3.4.1",
        "chai-as-promised": "^5.2.0",
        "coveralls": "^2.11.6",
        "del": "^2.2.0",
        "envify": "^3.4.0",
        "fbjs-scripts": "^0.5.0",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.1.1",
        "gulp-eslint": "^1.1.1",
        "gulp-if": "^2.0.0",
        "gulp-rename": "^1.2.2",
        "gulp-uglify": "^1.5.1",
        "istanbul": "^1.0.0-alpha.2",
        "mocha": "^2.3.4",
        "mocha-lcov-reporter": "^1.0.0",
        "mocha-phantomjs": "^4.0.2",
        "sinon": "^1.17.2",
        "sinon-chai": "^2.8.0",
        "require-dir": "^0.3.0",
        "run-sequence": "^1.1.5",
        "vinyl-buffer": "^1.0.0",
        "vinyl-source-stream": "^1.1.0"
    },
    "scripts": {
        "test_some": "mocha --require babelhook --reporter spec --timeout 1000",
        "test_browser": "gulp build:browser:tests && mocha-phantomjs --reporter spec browser_tests.html",
        "test": "mocha --require babelhook --reporter spec --timeout 1000 test/both test/node",
        "coverage": "./node_modules/.bin/babel-node ./node_modules/istanbul/lib/cli cover _mocha test/both test/node -- -u exports -R spec && open coverage/lcov-report/index.html",
        "coveralls": "./node_modules/.bin/babel-node ./node_modules/istanbul/lib/cli cover _mocha test/both test/node --report lcovonly -- -R spec && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js ./lib && rm -rf ./coverage"
    },
    "main": "index.js",
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
