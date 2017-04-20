# npmdoc-mongoose

#### api documentation for  [mongoose (v4.9.5)](http://mongoosejs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-mongoose.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mongoose) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongoose.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongoose)

#### Mongoose MongoDB ODM

[![NPM](https://nodei.co/npm/mongoose.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mongoose)

- [https://npmdoc.github.io/node-npmdoc-mongoose/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mongoose/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongoose/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongoose/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mongoose/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mongoose/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guillermo Rauch"
    },
    "browser": "lib/browser.js",
    "browserDependencies": {
        "browserify": "4.1.10",
        "chai": "3.5.0",
        "karma": "0.12.16",
        "karma-chai": "0.1.0",
        "karma-mocha": "0.1.4",
        "karma-chrome-launcher": "0.1.4",
        "karma-sauce-launcher": "0.2.8"
    },
    "bugs": {
        "url": "https://github.com/Automattic/mongoose/issues/new"
    },
    "dependencies": {
        "async": "2.1.4",
        "bson": "~1.0.4",
        "hooks-fixed": "2.0.0",
        "kareem": "1.2.1",
        "mongodb": "2.2.25",
        "mpath": "0.2.1",
        "mpromise": "0.5.5",
        "mquery": "2.3.0",
        "ms": "0.7.2",
        "muri": "1.2.1",
        "regexp-clone": "0.0.1",
        "sliced": "1.0.1"
    },
    "description": "Mongoose MongoDB ODM",
    "devDependencies": {
        "acquit": "0.4.1",
        "acquit-ignore": "0.0.3",
        "benchmark": "2.1.2",
        "bluebird": "3.4.6",
        "co": "4.6.0",
        "dox": "0.3.1",
        "eslint": "2.4.0",
        "highlight.js": "7.0.1",
        "istanbul": "0.4.4",
        "jade": "0.26.3",
        "lodash": "4.16.6",
        "markdown": "0.3.1",
        "marked": "0.3.6",
        "mocha": "3.2.0",
        "mongoose-long": "0.1.1",
        "node-static": "0.7.7",
        "power-assert": "1.4.1",
        "q": "1.4.1",
        "tbd": "0.6.4",
        "uglify-js": "2.7.0",
        "uuid": "2.0.3",
        "validator": "5.4.0"
    },
    "directories": {
        "lib": "./lib/mongoose"
    },
    "dist": {
        "shasum": "856b856700032748dd68122cb0371f8980442975",
        "tarball": "https://registry.npmjs.org/mongoose/-/mongoose-4.9.5.tgz"
    },
    "engines": {
        "node": ">=0.6.19"
    },
    "gitHead": "e5390b16cc9251687cbaf6f3712cf646fab3f854",
    "homepage": "http://mongoosejs.com",
    "keywords": [
        "mongodb",
        "document",
        "model",
        "schema",
        "database",
        "odm",
        "data",
        "datastore",
        "query",
        "nosql",
        "orm",
        "db"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "rauchg"
        },
        {
            "name": "tjholowaychuk"
        },
        {
            "name": "aaron"
        },
        {
            "name": "vkarpov15"
        },
        {
            "name": "defunctzombie"
        }
    ],
    "name": "mongoose",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/Automattic/mongoose.git"
    },
    "scripts": {
        "fix-lint": "eslint . --fix",
        "install-browser": "npm install 'node format_deps.js'",
        "lint": "eslint . --quiet",
        "test": "mocha test/*.test.js test/**/*.test.js",
        "test-cov": "istanbul cover --report text --report html _mocha test/*.test.js"
    },
    "version": "4.9.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
