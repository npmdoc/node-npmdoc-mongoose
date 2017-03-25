# api documentation for  [mongoose (v4.9.1)](http://mongoosejs.com)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongoose.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongoose)
#### Mongoose MongoDB ODM

[![NPM](https://nodei.co/npm/mongoose.png?downloads=true)](https://www.npmjs.com/package/mongoose)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongoose/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mongoose_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongoose/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-mongoose/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Guillermo Rauch",
        "email": "guillermo@learnboost.com"
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
        "url": "https://github.com/Automattic/mongoose/issues/new",
        "email": "mongoose-orm@googlegroups.com"
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
        "shasum": "e621d9e7356f46d1e39980a71063857405fa9099",
        "tarball": "https://registry.npmjs.org/mongoose/-/mongoose-4.9.1.tgz"
    },
    "engines": {
        "node": ">=0.6.19"
    },
    "gitHead": "4f864cf5a8dbb843883a2c097b69038149938718",
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
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        },
        {
            "name": "tjholowaychuk",
            "email": "tj@vision-media.ca"
        },
        {
            "name": "aaron",
            "email": "aaron.heckmann+github@gmail.com"
        },
        {
            "name": "vkarpov15",
            "email": "val@karpov.io"
        },
        {
            "name": "defunctzombie",
            "email": "shtylman@gmail.com"
        }
    ],
    "name": "mongoose",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/Automattic/mongoose.git"
    },
    "scripts": {
        "fix-lint": "eslint . --fix",
        "install-browser": "npm install 'node format_deps.js'",
        "posttest": "eslint . --quiet",
        "test": "mocha test/*.test.js test/**/*.test.js",
        "test-cov": "istanbul cover --report text --report html _mocha test/*.test.js"
    },
    "version": "4.9.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mongoose](#apidoc.module.mongoose)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>ES6Promise ()](#apidoc.element.mongoose.ES6Promise)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>aggregate ()](#apidoc.element.mongoose.aggregate)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>browserDocument (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>collection (name, conn, opts)](#apidoc.element.mongoose.collection)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>connection (base)](#apidoc.element.mongoose.connection)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>document (obj, fields, skipId)](#apidoc.element.mongoose.document)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>error (msg)](#apidoc.element.mongoose.error)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>model (doc, fields, skipId)](#apidoc.element.mongoose.model)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>promise (fn)](#apidoc.element.mongoose.promise)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>query (conditions, options, model, collection)](#apidoc.element.mongoose.query)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>querycursor (query, options)](#apidoc.element.mongoose.querycursor)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>querystream (query, options)](#apidoc.element.mongoose.querystream)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>schema (obj, options)](#apidoc.element.mongoose.schema)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>schematype (path, options, instance)](#apidoc.element.mongoose.schematype)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>statemachine ()](#apidoc.element.mongoose.statemachine)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>virtualtype (options, name)](#apidoc.element.mongoose.virtualtype)
1.  object <span class="apidocSignatureSpan">mongoose.</span>aggregate.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>browser
1.  object <span class="apidocSignatureSpan">mongoose.</span>browserDocument.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>collection.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>connection.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>connections
1.  object <span class="apidocSignatureSpan">mongoose.</span>document.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>drivers
1.  object <span class="apidocSignatureSpan">mongoose.</span>error.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>model.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>modelSchemas
1.  object <span class="apidocSignatureSpan">mongoose.</span>models
1.  object <span class="apidocSignatureSpan">mongoose.</span>options
1.  object <span class="apidocSignatureSpan">mongoose.</span>plugins
1.  object <span class="apidocSignatureSpan">mongoose.</span>promise.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>promise_provider
1.  object <span class="apidocSignatureSpan">mongoose.</span>query.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>querycursor.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>queryhelpers
1.  object <span class="apidocSignatureSpan">mongoose.</span>querystream.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>schema.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>schematype.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>statemachine.prototype
1.  object <span class="apidocSignatureSpan">mongoose.</span>types
1.  object <span class="apidocSignatureSpan">mongoose.</span>utils
1.  object <span class="apidocSignatureSpan">mongoose.</span>virtualtype.prototype

#### [module mongoose.ES6Promise](#apidoc.module.mongoose.ES6Promise)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>ES6Promise ()](#apidoc.element.mongoose.ES6Promise.ES6Promise)
1.  [function <span class="apidocSignatureSpan">mongoose.ES6Promise.</span>use (Promise)](#apidoc.element.mongoose.ES6Promise.use)

#### [module mongoose.aggregate](#apidoc.module.mongoose.aggregate)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>aggregate ()](#apidoc.element.mongoose.aggregate.aggregate)

#### [module mongoose.aggregate.prototype](#apidoc.module.mongoose.aggregate.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>addCursorFlag (flag, value)](#apidoc.element.mongoose.aggregate.prototype.addCursorFlag)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>allowDiskUse (value)](#apidoc.element.mongoose.aggregate.prototype.allowDiskUse)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>append ()](#apidoc.element.mongoose.aggregate.prototype.append)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>collation (collation)](#apidoc.element.mongoose.aggregate.prototype.collation)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>cursor (options)](#apidoc.element.mongoose.aggregate.prototype.cursor)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>exec (callback)](#apidoc.element.mongoose.aggregate.prototype.exec)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>explain (callback)](#apidoc.element.mongoose.aggregate.prototype.explain)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>facet (options)](#apidoc.element.mongoose.aggregate.prototype.facet)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>graphLookup (options)](#apidoc.element.mongoose.aggregate.prototype.graphLookup)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>group (arg)](#apidoc.element.mongoose.aggregate.prototype.group)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>limit (arg)](#apidoc.element.mongoose.aggregate.prototype.limit)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>lookup (options)](#apidoc.element.mongoose.aggregate.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>match (arg)](#apidoc.element.mongoose.aggregate.prototype.match)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>model (model)](#apidoc.element.mongoose.aggregate.prototype.model)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>near (arg)](#apidoc.element.mongoose.aggregate.prototype.near)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>out (arg)](#apidoc.element.mongoose.aggregate.prototype.out)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>project (arg)](#apidoc.element.mongoose.aggregate.prototype.project)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>read (pref, tags)](#apidoc.element.mongoose.aggregate.prototype.read)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>sample (size)](#apidoc.element.mongoose.aggregate.prototype.sample)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>skip (arg)](#apidoc.element.mongoose.aggregate.prototype.skip)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>sort (arg)](#apidoc.element.mongoose.aggregate.prototype.sort)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>then (resolve, reject)](#apidoc.element.mongoose.aggregate.prototype.then)
1.  [function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>unwind ()](#apidoc.element.mongoose.aggregate.prototype.unwind)

#### [module mongoose.browser](#apidoc.module.mongoose.browser)
1.  [function <span class="apidocSignatureSpan">mongoose.browser.</span>Document (obj, fields, skipId)](#apidoc.element.mongoose.browser.Document)
1.  [function <span class="apidocSignatureSpan">mongoose.browser.</span>Error (msg)](#apidoc.element.mongoose.browser.Error)
1.  [function <span class="apidocSignatureSpan">mongoose.browser.</span>Schema (obj, options)](#apidoc.element.mongoose.browser.Schema)
1.  [function <span class="apidocSignatureSpan">mongoose.browser.</span>SchemaType (path, options, instance)](#apidoc.element.mongoose.browser.SchemaType)
1.  [function <span class="apidocSignatureSpan">mongoose.browser.</span>VirtualType (options, name)](#apidoc.element.mongoose.browser.VirtualType)
1.  object <span class="apidocSignatureSpan">mongoose.browser.</span>PromiseProvider
1.  object <span class="apidocSignatureSpan">mongoose.browser.</span>Types
1.  object <span class="apidocSignatureSpan">mongoose.browser.</span>utils

#### [module mongoose.browserDocument](#apidoc.module.mongoose.browserDocument)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>browserDocument (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument.browserDocument)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>ValidationError (instance)](#apidoc.element.mongoose.browserDocument.ValidationError)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>addListener ()](#apidoc.element.mongoose.browserDocument.addListener)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>emit ()](#apidoc.element.mongoose.browserDocument.emit)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>listeners ()](#apidoc.element.mongoose.browserDocument.listeners)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>on ()](#apidoc.element.mongoose.browserDocument.on)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>once ()](#apidoc.element.mongoose.browserDocument.once)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>removeAllListeners ()](#apidoc.element.mongoose.browserDocument.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>removeListener ()](#apidoc.element.mongoose.browserDocument.removeListener)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>setMaxListeners ()](#apidoc.element.mongoose.browserDocument.setMaxListeners)

#### [module mongoose.browserDocument.prototype](#apidoc.module.mongoose.browserDocument.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.browserDocument.prototype.</span>constructor (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument.prototype.constructor)

#### [module mongoose.collection](#apidoc.module.mongoose.collection)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>collection (name, conn, opts)](#apidoc.element.mongoose.collection.collection)

#### [module mongoose.collection.prototype](#apidoc.module.mongoose.collection.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>addQueue (name, args)](#apidoc.element.mongoose.collection.prototype.addQueue)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>doQueue ()](#apidoc.element.mongoose.collection.prototype.doQueue)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>ensureIndex ()](#apidoc.element.mongoose.collection.prototype.ensureIndex)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>find ()](#apidoc.element.mongoose.collection.prototype.find)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>findAndModify ()](#apidoc.element.mongoose.collection.prototype.findAndModify)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>findOne ()](#apidoc.element.mongoose.collection.prototype.findOne)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>getIndexes ()](#apidoc.element.mongoose.collection.prototype.getIndexes)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>insert ()](#apidoc.element.mongoose.collection.prototype.insert)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>mapReduce ()](#apidoc.element.mongoose.collection.prototype.mapReduce)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>onClose ()](#apidoc.element.mongoose.collection.prototype.onClose)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>onOpen ()](#apidoc.element.mongoose.collection.prototype.onOpen)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>save ()](#apidoc.element.mongoose.collection.prototype.save)
1.  [function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>update ()](#apidoc.element.mongoose.collection.prototype.update)

#### [module mongoose.connection](#apidoc.module.mongoose.connection)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>connection (base)](#apidoc.element.mongoose.connection.connection)
1.  object <span class="apidocSignatureSpan">mongoose.connection.</span>STATES

#### [module mongoose.connection.prototype](#apidoc.module.mongoose.connection.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>_close (callback)](#apidoc.element.mongoose.connection.prototype._close)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>_open (emit, callback)](#apidoc.element.mongoose.connection.prototype._open)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>authMechanismDoesNotRequirePassword ()](#apidoc.element.mongoose.connection.prototype.authMechanismDoesNotRequirePassword)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>close (callback)](#apidoc.element.mongoose.connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>collection (name, options)](#apidoc.element.mongoose.connection.prototype.collection)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>dropDatabase (callback)](#apidoc.element.mongoose.connection.prototype.dropDatabase)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>error (err, callback)](#apidoc.element.mongoose.connection.prototype.error)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>model (name, schema, collection)](#apidoc.element.mongoose.connection.prototype.model)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>modelNames ()](#apidoc.element.mongoose.connection.prototype.modelNames)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>onClose ()](#apidoc.element.mongoose.connection.prototype.onClose)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>onOpen (callback)](#apidoc.element.mongoose.connection.prototype.onOpen)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>open (host, database, port, options, callback)](#apidoc.element.mongoose.connection.prototype.open)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>openSet (uris, database, options, callback)](#apidoc.element.mongoose.connection.prototype.openSet)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>optionsProvideAuthenticationData (options)](#apidoc.element.mongoose.connection.prototype.optionsProvideAuthenticationData)
1.  [function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>shouldAuthenticate ()](#apidoc.element.mongoose.connection.prototype.shouldAuthenticate)

#### [module mongoose.document](#apidoc.module.mongoose.document)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>document (obj, fields, skipId)](#apidoc.element.mongoose.document.document)
1.  [function <span class="apidocSignatureSpan">mongoose.document.</span>ValidationError (instance)](#apidoc.element.mongoose.document.ValidationError)
1.  [function <span class="apidocSignatureSpan">mongoose.document.</span>_lazySetupHooks (proto, methodName, errorCb)](#apidoc.element.mongoose.document._lazySetupHooks)
1.  [function <span class="apidocSignatureSpan">mongoose.document.</span>removePost (name, fnToRemove)](#apidoc.element.mongoose.document.removePost)
1.  [function <span class="apidocSignatureSpan">mongoose.document.</span>removePre (name, fnToRemove)](#apidoc.element.mongoose.document.removePre)

#### [module mongoose.document.prototype](#apidoc.module.mongoose.document.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>_lazySetupHooks (proto, methodName, errorCb)](#apidoc.element.mongoose.document.prototype._lazySetupHooks)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>addListener ()](#apidoc.element.mongoose.document.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>depopulate (path)](#apidoc.element.mongoose.document.prototype.depopulate)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>emit ()](#apidoc.element.mongoose.document.prototype.emit)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>equals (doc)](#apidoc.element.mongoose.document.prototype.equals)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>execPopulate ()](#apidoc.element.mongoose.document.prototype.execPopulate)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>get (path, type)](#apidoc.element.mongoose.document.prototype.get)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>getValue (path)](#apidoc.element.mongoose.document.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>init (doc, opts, fn)](#apidoc.element.mongoose.document.prototype.init)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>inspect (options)](#apidoc.element.mongoose.document.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>invalidate (path, err, val, kind)](#apidoc.element.mongoose.document.prototype.invalidate)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isDirectModified (path)](#apidoc.element.mongoose.document.prototype.isDirectModified)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isInit (path)](#apidoc.element.mongoose.document.prototype.isInit)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isModified (paths)](#apidoc.element.mongoose.document.prototype.isModified)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isSelected (path)](#apidoc.element.mongoose.document.prototype.isSelected)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>listeners ()](#apidoc.element.mongoose.document.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>markModified (path)](#apidoc.element.mongoose.document.prototype.markModified)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>modifiedPaths ()](#apidoc.element.mongoose.document.prototype.modifiedPaths)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>on ()](#apidoc.element.mongoose.document.prototype.on)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>once ()](#apidoc.element.mongoose.document.prototype.once)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>populate ()](#apidoc.element.mongoose.document.prototype.populate)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>populated (path, val, options)](#apidoc.element.mongoose.document.prototype.populated)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removeAllListeners ()](#apidoc.element.mongoose.document.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removeListener ()](#apidoc.element.mongoose.document.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removePost (name, fnToRemove)](#apidoc.element.mongoose.document.prototype.removePost)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removePre (name, fnToRemove)](#apidoc.element.mongoose.document.prototype.removePre)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>set (path, val, type, options)](#apidoc.element.mongoose.document.prototype.set)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>setMaxListeners ()](#apidoc.element.mongoose.document.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>setValue (path, val)](#apidoc.element.mongoose.document.prototype.setValue)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toBSON ()](#apidoc.element.mongoose.document.prototype.toBSON)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toJSON (options)](#apidoc.element.mongoose.document.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toObject (options)](#apidoc.element.mongoose.document.prototype.toObject)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toString ()](#apidoc.element.mongoose.document.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>unmarkModified (path)](#apidoc.element.mongoose.document.prototype.unmarkModified)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>update ()](#apidoc.element.mongoose.document.prototype.update)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>validate (options, callback)](#apidoc.element.mongoose.document.prototype.validate)
1.  [function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>validateSync (pathsToValidate)](#apidoc.element.mongoose.document.prototype.validateSync)

#### [module mongoose.drivers](#apidoc.module.mongoose.drivers)
1.  [function <span class="apidocSignatureSpan">mongoose.drivers.</span>Binary (buffer, subType)](#apidoc.element.mongoose.drivers.Binary)
1.  [function <span class="apidocSignatureSpan">mongoose.drivers.</span>ObjectId (id)](#apidoc.element.mongoose.drivers.ObjectId)
1.  [function <span class="apidocSignatureSpan">mongoose.drivers.</span>ReadPreference (pref, tags)](#apidoc.element.mongoose.drivers.ReadPreference)

#### [module mongoose.error](#apidoc.module.mongoose.error)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>error (msg)](#apidoc.element.mongoose.error.error)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>CastError (type, value, path, reason)](#apidoc.element.mongoose.error.CastError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>DivergentArrayError (paths)](#apidoc.element.mongoose.error.DivergentArrayError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>DocumentNotFoundError (query)](#apidoc.element.mongoose.error.DocumentNotFoundError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>MissingSchemaError (name)](#apidoc.element.mongoose.error.MissingSchemaError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>OverwriteModelError (name)](#apidoc.element.mongoose.error.OverwriteModelError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>ValidationError (instance)](#apidoc.element.mongoose.error.ValidationError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>ValidatorError (properties)](#apidoc.element.mongoose.error.ValidatorError)
1.  [function <span class="apidocSignatureSpan">mongoose.error.</span>VersionError (doc)](#apidoc.element.mongoose.error.VersionError)
1.  object <span class="apidocSignatureSpan">mongoose.error.</span>Messages
1.  object <span class="apidocSignatureSpan">mongoose.error.</span>messages

#### [module mongoose.error.prototype](#apidoc.module.mongoose.error.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.error.prototype.</span>constructor ()](#apidoc.element.mongoose.error.prototype.constructor)

#### [module mongoose.model](#apidoc.module.mongoose.model)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>model (doc, fields, skipId)](#apidoc.element.mongoose.model.model)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>__subclass (conn, schema, collection)](#apidoc.element.mongoose.model.__subclass)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>_getSchema (path)](#apidoc.element.mongoose.model._getSchema)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>addListener (type, listener)](#apidoc.element.mongoose.model.addListener)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>aggregate ()](#apidoc.element.mongoose.model.aggregate)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>bulkWrite (ops, options, callback)](#apidoc.element.mongoose.model.bulkWrite)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>compile (name, schema, collectionName, connection, base)](#apidoc.element.mongoose.model.compile)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>count (conditions, callback)](#apidoc.element.mongoose.model.count)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>create (doc, callback)](#apidoc.element.mongoose.model.create)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>deleteMany (conditions, callback)](#apidoc.element.mongoose.model.deleteMany)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>deleteOne (conditions, callback)](#apidoc.element.mongoose.model.deleteOne)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>discriminator (name, schema)](#apidoc.element.mongoose.model.discriminator)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>distinct (field, conditions, callback)](#apidoc.element.mongoose.model.distinct)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>emit (type)](#apidoc.element.mongoose.model.emit)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>ensureIndexes (options, callback)](#apidoc.element.mongoose.model.ensureIndexes)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>eventNames ()](#apidoc.element.mongoose.model.eventNames)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>find (conditions, projection, options, callback)](#apidoc.element.mongoose.model.find)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findById (id, projection, options, callback)](#apidoc.element.mongoose.model.findById)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findByIdAndRemove (id, options, callback)](#apidoc.element.mongoose.model.findByIdAndRemove)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findByIdAndUpdate (id, update, options, callback)](#apidoc.element.mongoose.model.findByIdAndUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findOne (conditions, projection, options, callback)](#apidoc.element.mongoose.model.findOne)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findOneAndRemove (conditions, options, callback)](#apidoc.element.mongoose.model.findOneAndRemove)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>findOneAndUpdate (conditions, update, options, callback)](#apidoc.element.mongoose.model.findOneAndUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>geoNear (near, options, callback)](#apidoc.element.mongoose.model.geoNear)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>geoSearch (conditions, options, callback)](#apidoc.element.mongoose.model.geoSearch)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>getMaxListeners ()](#apidoc.element.mongoose.model.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>hydrate (obj)](#apidoc.element.mongoose.model.hydrate)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>init ()](#apidoc.element.mongoose.model.init)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>insertMany (arr, options, callback)](#apidoc.element.mongoose.model.insertMany)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>listenerCount (type)](#apidoc.element.mongoose.model.listenerCount)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>listeners (type)](#apidoc.element.mongoose.model.listeners)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>mapReduce (o, callback)](#apidoc.element.mongoose.model.mapReduce)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>on (type, listener)](#apidoc.element.mongoose.model.on)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>once (type, listener)](#apidoc.element.mongoose.model.once)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>populate (docs, paths, callback)](#apidoc.element.mongoose.model.populate)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>prependListener (type, listener)](#apidoc.element.mongoose.model.prependListener)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>prependOnceListener (type, listener)](#apidoc.element.mongoose.model.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>remove (conditions, callback)](#apidoc.element.mongoose.model.remove)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>removeAllListeners (type)](#apidoc.element.mongoose.model.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>removeListener (type, listener)](#apidoc.element.mongoose.model.removeListener)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>replaceOne (conditions, doc, options, callback)](#apidoc.element.mongoose.model.replaceOne)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>setMaxListeners (n)](#apidoc.element.mongoose.model.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>update (conditions, doc, options, callback)](#apidoc.element.mongoose.model.update)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>updateMany (conditions, doc, options, callback)](#apidoc.element.mongoose.model.updateMany)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>updateOne (conditions, doc, options, callback)](#apidoc.element.mongoose.model.updateOne)
1.  [function <span class="apidocSignatureSpan">mongoose.model.</span>where (path, val)](#apidoc.element.mongoose.model.where)
1.  undefined <span class="apidocSignatureSpan">mongoose.model.</span>domain

#### [module mongoose.model.prototype](#apidoc.module.mongoose.model.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>increment ()](#apidoc.element.mongoose.model.prototype.increment)
1.  [function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>model (name)](#apidoc.element.mongoose.model.prototype.model)
1.  [function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>remove (options, fn)](#apidoc.element.mongoose.model.prototype.remove)
1.  [function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>save (options, fn)](#apidoc.element.mongoose.model.prototype.save)

#### [module mongoose.promise](#apidoc.module.mongoose.promise)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>promise (fn)](#apidoc.element.mongoose.promise.promise)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.</span>ES6 (resolver)](#apidoc.element.mongoose.promise.ES6)
1.  string <span class="apidocSignatureSpan">mongoose.promise.</span>FAILURE
1.  string <span class="apidocSignatureSpan">mongoose.promise.</span>SUCCESS

#### [module mongoose.promise.prototype](#apidoc.module.mongoose.promise.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addBack (fn)](#apidoc.element.mongoose.promise.prototype.addBack)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addCallback (fn)](#apidoc.element.mongoose.promise.prototype.addCallback)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addErrback (fn)](#apidoc.element.mongoose.promise.prototype.addErrback)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>catch (onReject)](#apidoc.element.mongoose.promise.prototype.catch)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>complete ()](#apidoc.element.mongoose.promise.prototype.complete)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>error (err)](#apidoc.element.mongoose.promise.prototype.error)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>resolve (err)](#apidoc.element.mongoose.promise.prototype.resolve)
1.  [function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>then ()](#apidoc.element.mongoose.promise.prototype.then)

#### [module mongoose.promise_provider](#apidoc.module.mongoose.promise_provider)
1.  [function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>_promise (fn)](#apidoc.element.mongoose.promise_provider._promise)
1.  [function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>get ()](#apidoc.element.mongoose.promise_provider.get)
1.  [function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>reset ()](#apidoc.element.mongoose.promise_provider.reset)
1.  [function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>set (lib)](#apidoc.element.mongoose.promise_provider.set)

#### [module mongoose.query](#apidoc.module.mongoose.query)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>query (conditions, options, model, collection)](#apidoc.element.mongoose.query.query)
1.  object <span class="apidocSignatureSpan">mongoose.query.</span>base

#### [module mongoose.query.prototype](#apidoc.module.mongoose.query.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_applyPaths ()](#apidoc.element.mongoose.query.prototype._applyPaths)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_castFields (fields)](#apidoc.element.mongoose.query.prototype._castFields)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_castUpdate (obj, overwrite)](#apidoc.element.mongoose.query.prototype._castUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_count (callback)](#apidoc.element.mongoose.query.prototype._count)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_execUpdate (callback)](#apidoc.element.mongoose.query.prototype._execUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_find (callback)](#apidoc.element.mongoose.query.prototype._find)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findAndModify (type, callback)](#apidoc.element.mongoose.query.prototype._findAndModify)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOne (callback)](#apidoc.element.mongoose.query.prototype._findOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOneAndRemove (callback)](#apidoc.element.mongoose.query.prototype._findOneAndRemove)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOneAndUpdate (callback)](#apidoc.element.mongoose.query.prototype._findOneAndUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_mergeUpdate (doc)](#apidoc.element.mongoose.query.prototype._mergeUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_optionsForExec (model)](#apidoc.element.mongoose.query.prototype._optionsForExec)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_replaceOne (callback)](#apidoc.element.mongoose.query.prototype._replaceOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateForExec ()](#apidoc.element.mongoose.query.prototype._updateForExec)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateMany (callback)](#apidoc.element.mongoose.query.prototype._updateMany)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateOne (callback)](#apidoc.element.mongoose.query.prototype._updateOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>box (ll, ur)](#apidoc.element.mongoose.query.prototype.box)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>cast (model, obj)](#apidoc.element.mongoose.query.prototype.cast)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>catch (reject)](#apidoc.element.mongoose.query.prototype.catch)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>center ()](#apidoc.element.mongoose.query.prototype.center)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>centerSphere ()](#apidoc.element.mongoose.query.prototype.centerSphere)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>collation (value)](#apidoc.element.mongoose.query.prototype.collation)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>constructor (conditions, options, model, collection)](#apidoc.element.mongoose.query.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>count (conditions, callback)](#apidoc.element.mongoose.query.prototype.count)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>cursor (opts)](#apidoc.element.mongoose.query.prototype.cursor)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>deleteMany (cond, callback)](#apidoc.element.mongoose.query.prototype.deleteMany)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>deleteOne (cond, callback)](#apidoc.element.mongoose.query.prototype.deleteOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>distinct (field, conditions, callback)](#apidoc.element.mongoose.query.prototype.distinct)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>exec (op, callback)](#apidoc.element.mongoose.query.prototype.exec)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>find (conditions, callback)](#apidoc.element.mongoose.query.prototype.find)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOne (conditions, projection, options, callback)](#apidoc.element.mongoose.query.prototype.findOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOneAndRemove (conditions, options, callback)](#apidoc.element.mongoose.query.prototype.findOneAndRemove)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOneAndUpdate (criteria, doc, options, callback)](#apidoc.element.mongoose.query.prototype.findOneAndUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>getQuery ()](#apidoc.element.mongoose.query.prototype.getQuery)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>getUpdate ()](#apidoc.element.mongoose.query.prototype.getUpdate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>lean (v)](#apidoc.element.mongoose.query.prototype.lean)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>maxscan (v)](#apidoc.element.mongoose.query.prototype.maxscan)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>merge (source)](#apidoc.element.mongoose.query.prototype.merge)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>mongooseOptions (v)](#apidoc.element.mongoose.query.prototype.mongooseOptions)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>near ()](#apidoc.element.mongoose.query.prototype.near)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>nearSphere ()](#apidoc.element.mongoose.query.prototype.nearSphere)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>populate ()](#apidoc.element.mongoose.query.prototype.populate)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>read (pref, tags)](#apidoc.element.mongoose.query.prototype.read)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>remove (cond, callback)](#apidoc.element.mongoose.query.prototype.remove)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>replaceOne (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.replaceOne)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>setOptions (options, overwrite)](#apidoc.element.mongoose.query.prototype.setOptions)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>sort (arg)](#apidoc.element.mongoose.query.prototype.sort)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>stream ()](#apidoc.element.mongoose.query.prototype.stream)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>tailable (val, opts)](#apidoc.element.mongoose.query.prototype.tailable)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>then (resolve, reject)](#apidoc.element.mongoose.query.prototype.then)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>toConstructor ()](#apidoc.element.mongoose.query.prototype.toConstructor)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>update (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.update)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>updateMany (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.updateMany)
1.  [function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>updateOne (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.updateOne)
1.  object <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_conditions
1.  object <span class="apidocSignatureSpan">mongoose.query.prototype.</span>options

#### [module mongoose.querycursor](#apidoc.module.mongoose.querycursor)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>querycursor (query, options)](#apidoc.element.mongoose.querycursor.querycursor)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.</span>super_ (options)](#apidoc.element.mongoose.querycursor.super_)

#### [module mongoose.querycursor.prototype](#apidoc.module.mongoose.querycursor.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>_markError (error)](#apidoc.element.mongoose.querycursor.prototype._markError)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>_read ()](#apidoc.element.mongoose.querycursor.prototype._read)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>close (callback)](#apidoc.element.mongoose.querycursor.prototype.close)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>eachAsync (fn, callback)](#apidoc.element.mongoose.querycursor.prototype.eachAsync)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>map (fn)](#apidoc.element.mongoose.querycursor.prototype.map)
1.  [function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>next (callback)](#apidoc.element.mongoose.querycursor.prototype.next)

#### [module mongoose.queryhelpers](#apidoc.module.mongoose.queryhelpers)
1.  [function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>applyPaths (fields, schema)](#apidoc.element.mongoose.queryhelpers.applyPaths)
1.  [function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>createModel (model, doc, fields)](#apidoc.element.mongoose.queryhelpers.createModel)
1.  [function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>preparePopulationOptions (query, options)](#apidoc.element.mongoose.queryhelpers.preparePopulationOptions)
1.  [function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>preparePopulationOptionsMQ (query, options)](#apidoc.element.mongoose.queryhelpers.preparePopulationOptionsMQ)

#### [module mongoose.querystream](#apidoc.module.mongoose.querystream)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>querystream (query, options)](#apidoc.element.mongoose.querystream.querystream)

#### [module mongoose.querystream.prototype](#apidoc.module.mongoose.querystream.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>__next ()](#apidoc.element.mongoose.querystream.prototype.__next)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_init ()](#apidoc.element.mongoose.querystream.prototype._init)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_next ()](#apidoc.element.mongoose.querystream.prototype._next)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_onNextObject (err, doc)](#apidoc.element.mongoose.querystream.prototype._onNextObject)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>destroy (err)](#apidoc.element.mongoose.querystream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>pause ()](#apidoc.element.mongoose.querystream.prototype.pause)
1.  [function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>resume ()](#apidoc.element.mongoose.querystream.prototype.resume)

#### [module mongoose.schema](#apidoc.module.mongoose.schema)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>schema (obj, options)](#apidoc.element.mongoose.schema.schema)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.</span>ObjectId (key, options)](#apidoc.element.mongoose.schema.ObjectId)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.</span>interpretAsType (path, obj, options)](#apidoc.element.mongoose.schema.interpretAsType)
1.  object <span class="apidocSignatureSpan">mongoose.schema.</span>Types
1.  object <span class="apidocSignatureSpan">mongoose.schema.</span>reserved

#### [module mongoose.schema.prototype](#apidoc.module.mongoose.schema.prototype)
1.  boolean <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>instanceOfSchema
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getPathType (path)](#apidoc.element.mongoose.schema.prototype._getPathType)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getSchema (path)](#apidoc.element.mongoose.schema.prototype._getSchema)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getVirtual (name)](#apidoc.element.mongoose.schema.prototype._getVirtual)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>add (obj, prefix)](#apidoc.element.mongoose.schema.prototype.add)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>clone ()](#apidoc.element.mongoose.schema.prototype.clone)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>constructor (obj, options)](#apidoc.element.mongoose.schema.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>defaultOptions (options)](#apidoc.element.mongoose.schema.prototype.defaultOptions)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>eachPath (fn)](#apidoc.element.mongoose.schema.prototype.eachPath)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>get (key)](#apidoc.element.mongoose.schema.prototype.get)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>hasMixedParent (path)](#apidoc.element.mongoose.schema.prototype.hasMixedParent)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>index (fields, options)](#apidoc.element.mongoose.schema.prototype.index)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>indexedPaths ()](#apidoc.element.mongoose.schema.prototype.indexedPaths)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>indexes ()](#apidoc.element.mongoose.schema.prototype.indexes)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>loadClass (model, virtualsOnly)](#apidoc.element.mongoose.schema.prototype.loadClass)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>method (name, fn)](#apidoc.element.mongoose.schema.prototype.method)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>path (path, obj)](#apidoc.element.mongoose.schema.prototype.path)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>pathType (path)](#apidoc.element.mongoose.schema.prototype.pathType)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>plugin (fn, opts)](#apidoc.element.mongoose.schema.prototype.plugin)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>post (method, fn)](#apidoc.element.mongoose.schema.prototype.post)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>pre ()](#apidoc.element.mongoose.schema.prototype.pre)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>queue (name, args)](#apidoc.element.mongoose.schema.prototype.queue)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>remove (path)](#apidoc.element.mongoose.schema.prototype.remove)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>requiredPaths (invalidate)](#apidoc.element.mongoose.schema.prototype.requiredPaths)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>set (key, value, _tags)](#apidoc.element.mongoose.schema.prototype.set)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>setupTimestamp (timestamps)](#apidoc.element.mongoose.schema.prototype.setupTimestamp)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>static (name, fn)](#apidoc.element.mongoose.schema.prototype.static)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>virtual (name, options)](#apidoc.element.mongoose.schema.prototype.virtual)
1.  [function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>virtualpath (name)](#apidoc.element.mongoose.schema.prototype.virtualpath)

#### [module mongoose.schematype](#apidoc.module.mongoose.schematype)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>schematype (path, options, instance)](#apidoc.element.mongoose.schematype.schematype)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.</span>CastError (type, value, path, reason)](#apidoc.element.mongoose.schematype.CastError)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.</span>ValidatorError (properties)](#apidoc.element.mongoose.schematype.ValidatorError)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.</span>_isRef (self, value, doc, init)](#apidoc.element.mongoose.schematype._isRef)

#### [module mongoose.schematype.prototype](#apidoc.module.mongoose.schematype.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>applyGetters (value, scope)](#apidoc.element.mongoose.schematype.prototype.applyGetters)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>applySetters (value, scope, init, priorVal, options)](#apidoc.element.mongoose.schematype.prototype.applySetters)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>castForQuery ($conditional, val)](#apidoc.element.mongoose.schematype.prototype.castForQuery)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>checkRequired (val)](#apidoc.element.mongoose.schematype.prototype.checkRequired)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>default (val)](#apidoc.element.mongoose.schematype.prototype.default)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>doValidate (value, fn, scope)](#apidoc.element.mongoose.schematype.prototype.doValidate)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>doValidateSync (value, scope)](#apidoc.element.mongoose.schematype.prototype.doValidateSync)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>get (fn)](#apidoc.element.mongoose.schematype.prototype.get)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>getDefault (scope, init)](#apidoc.element.mongoose.schematype.prototype.getDefault)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>index (options)](#apidoc.element.mongoose.schematype.prototype.index)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>required (required, message)](#apidoc.element.mongoose.schematype.prototype.required)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>select (val)](#apidoc.element.mongoose.schematype.prototype.select)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>set (fn)](#apidoc.element.mongoose.schematype.prototype.set)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>sparse (bool)](#apidoc.element.mongoose.schematype.prototype.sparse)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>text (bool)](#apidoc.element.mongoose.schematype.prototype.text)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>unique (bool)](#apidoc.element.mongoose.schematype.prototype.unique)
1.  [function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>validate (obj, message, type)](#apidoc.element.mongoose.schematype.prototype.validate)

#### [module mongoose.statemachine](#apidoc.module.mongoose.statemachine)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>statemachine ()](#apidoc.element.mongoose.statemachine.statemachine)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.</span>ctor ()](#apidoc.element.mongoose.statemachine.ctor)

#### [module mongoose.statemachine.prototype](#apidoc.module.mongoose.statemachine.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>_changeState (path, nextState)](#apidoc.element.mongoose.statemachine.prototype._changeState)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>_iter (iterMethod)](#apidoc.element.mongoose.statemachine.prototype._iter)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>clear (state)](#apidoc.element.mongoose.statemachine.prototype.clear)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>forEach ()](#apidoc.element.mongoose.statemachine.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>map ()](#apidoc.element.mongoose.statemachine.prototype.map)
1.  [function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>some ()](#apidoc.element.mongoose.statemachine.prototype.some)

#### [module mongoose.types](#apidoc.module.mongoose.types)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Array (values, path, doc)](#apidoc.element.mongoose.types.Array)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Buffer (value, encode, offset)](#apidoc.element.mongoose.types.Buffer)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Decimal128 (bytes)](#apidoc.element.mongoose.types.Decimal128)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Document (obj, parentArr, skipId, fields, index)](#apidoc.element.mongoose.types.Document)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>DocumentArray (values, path, doc)](#apidoc.element.mongoose.types.DocumentArray)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Embedded (obj, parentArr, skipId, fields, index)](#apidoc.element.mongoose.types.Embedded)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>ObjectId (id)](#apidoc.element.mongoose.types.ObjectId)
1.  [function <span class="apidocSignatureSpan">mongoose.types.</span>Subdocument (value, fields)](#apidoc.element.mongoose.types.Subdocument)

#### [module mongoose.utils](#apidoc.module.mongoose.utils)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>PopulateOptions (path, select, match, options, model, subPopulate)](#apidoc.element.mongoose.utils.PopulateOptions)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>args (args, slice, sliceEnd)](#apidoc.element.mongoose.utils.args)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>clone (obj, options)](#apidoc.element.mongoose.utils.clone)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>decorate (destination, source)](#apidoc.element.mongoose.utils.decorate)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>deepEqual (a, b)](#apidoc.element.mongoose.utils.deepEqual)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>each (arr, fn)](#apidoc.element.mongoose.utils.each)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>expires (object)](#apidoc.element.mongoose.utils.expires)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>getFunctionName (fn)](#apidoc.element.mongoose.utils.getFunctionName)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>getValue (path, obj, map)](#apidoc.element.mongoose.utils.getValue)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>isMongooseObject (v)](#apidoc.element.mongoose.utils.isMongooseObject)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>isNullOrUndefined (val)](#apidoc.element.mongoose.utils.isNullOrUndefined)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>isObject (arg)](#apidoc.element.mongoose.utils.isObject)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>merge (to, from, options)](#apidoc.element.mongoose.utils.merge)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>mergeClone (to, fromObj)](#apidoc.element.mongoose.utils.mergeClone)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>options (defaults, options)](#apidoc.element.mongoose.utils.options)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>populate (path, select, model, match, options, subPopulate)](#apidoc.element.mongoose.utils.populate)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>random ()](#apidoc.element.mongoose.utils.random)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>setValue (path, val, obj, map)](#apidoc.element.mongoose.utils.setValue)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>tick (callback)](#apidoc.element.mongoose.utils.tick)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>toCollectionName (name, options)](#apidoc.element.mongoose.utils.toCollectionName)
1.  [function <span class="apidocSignatureSpan">mongoose.utils.</span>toObject (obj)](#apidoc.element.mongoose.utils.toObject)
1.  object <span class="apidocSignatureSpan">mongoose.utils.</span>array
1.  object <span class="apidocSignatureSpan">mongoose.utils.</span>buffer
1.  object <span class="apidocSignatureSpan">mongoose.utils.</span>object
1.  object <span class="apidocSignatureSpan">mongoose.utils.</span>pluralization
1.  object <span class="apidocSignatureSpan">mongoose.utils.</span>uncountables

#### [module mongoose.virtualtype](#apidoc.module.mongoose.virtualtype)
1.  [function <span class="apidocSignatureSpan">mongoose.</span>virtualtype (options, name)](#apidoc.element.mongoose.virtualtype.virtualtype)

#### [module mongoose.virtualtype.prototype](#apidoc.module.mongoose.virtualtype.prototype)
1.  [function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>applyGetters (value, scope)](#apidoc.element.mongoose.virtualtype.prototype.applyGetters)
1.  [function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>applySetters (value, scope)](#apidoc.element.mongoose.virtualtype.prototype.applySetters)
1.  [function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>get (fn)](#apidoc.element.mongoose.virtualtype.prototype.get)
1.  [function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>set (fn)](#apidoc.element.mongoose.virtualtype.prototype.set)



# <a name="apidoc.module.mongoose"></a>[module mongoose](#apidoc.module.mongoose)

#### <a name="apidoc.element.mongoose.ES6Promise"></a>[function <span class="apidocSignatureSpan">mongoose.</span>ES6Promise ()](#apidoc.element.mongoose.ES6Promise)
- description and source-code
```javascript
function ES6Promise() {
  throw new Error('Can\'t use ES6 promise with mpromise style constructor');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.aggregate"></a>[function <span class="apidocSignatureSpan">mongoose.</span>aggregate ()](#apidoc.element.mongoose.aggregate)
- description and source-code
```javascript
function Aggregate() {
  this._pipeline = [];
  this._model = undefined;
  this.options = undefined;

  if (arguments.length === 1 && util.isArray(arguments[0])) {
    this.append.apply(this, arguments[0]);
  } else {
    this.append.apply(this, arguments);
  }
}
```
- example usage
```shell
...
* ####Example:
*
*     new Aggregate();
*     new Aggregate({ $project: { a: 1, b: 1 } });
*     new Aggregate({ $project: { a: 1, b: 1 } }, { $skip: 5 });
*     new Aggregate([{ $project: { a: 1, b: 1 } }, { $skip: 5 }]);
*
* Returned when calling Model.aggregate().
*
* ####Example:
*
*     Model
*     .aggregate({ $match: { age: { $gte: 21 }}})
*     .unwind('tags')
*     .exec(callback)
...
```

#### <a name="apidoc.element.mongoose.browserDocument"></a>[function <span class="apidocSignatureSpan">mongoose.</span>browserDocument (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument)
- description and source-code
```javascript
function Document(obj, schema, fields, skipId, skipInit) {
  if (!(this instanceof Document)) {
    return new Document(obj, schema, fields, skipId, skipInit);
  }


  if (utils.isObject(schema) && !schema.instanceOfSchema) {
    schema = new Schema(schema);
  }

  // When creating EmbeddedDocument, it already has the schema and he doesn't need the _id
  schema = this.schema || schema;

  // Generate ObjectId if it is missing, but it requires a scheme
  if (!this.schema && schema.options._id) {
    obj = obj || {};

    if (obj._id === undefined) {
      obj._id = new ObjectId();
    }
  }

  if (!schema) {
    throw new MongooseError.MissingSchemaError();
  }

  this.$__setSchema(schema);

  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = this.schema.options && this.schema.options.strict;
    this.$__.selected = fields;
  }

  var required = this.schema.requiredPaths();
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (!skipInit && obj) {
    this.init(obj);
  }

  this.$__registerHooksFromSchema();

  // apply methods
  for (var m in schema.methods) {
    this[m] = schema.methods[m];
  }
  // apply statics
  for (var s in schema.statics) {
    this[s] = schema.statics[s];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.collection"></a>[function <span class="apidocSignatureSpan">mongoose.</span>collection (name, conn, opts)](#apidoc.element.mongoose.collection)
- description and source-code
```javascript
function Collection(name, conn, opts) {
  if (opts === void 0) {
    opts = {};
  }
  if (opts.capped === void 0) {
    opts.capped = {};
  }

  opts.bufferCommands = undefined === opts.bufferCommands
      ? true
      : opts.bufferCommands;

  if (typeof opts.capped === 'number') {
    opts.capped = {size: opts.capped};
  }

  this.opts = opts;
  this.name = name;
  this.collectionName = name;
  this.conn = conn;
  this.queue = [];
  this.buffer = this.opts.bufferCommands;
  this.emitter = new EventEmitter();

  if (STATES.connected === this.conn.readyState) {
    this.onOpen();
  }
}
```
- example usage
```shell
...
model.prototype.$__setSchema(schema);

var collectionOptions = {
  bufferCommands: schema.options.bufferCommands,
  capped: schema.options.capped
};

model.prototype.collection = connection.collection(
    collectionName
    , collectionOptions
);

// apply methods and statics
applyMethods(model, schema);
applyStatics(model, schema);
...
```

#### <a name="apidoc.element.mongoose.connection"></a>[function <span class="apidocSignatureSpan">mongoose.</span>connection (base)](#apidoc.element.mongoose.connection)
- description and source-code
```javascript
function Connection(base) {
  this.base = base;
  this.collections = {};
  this.models = {};
  this.config = {autoIndex: true};
  this.replica = false;
  this.hosts = null;
  this.host = null;
  this.port = null;
  this.user = null;
  this.pass = null;
  this.name = null;
  this.options = null;
  this.otherDbs = [];
  this._readyState = STATES.disconnected;
  this._closeCalled = false;
  this._hasOpened = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document"></a>[function <span class="apidocSignatureSpan">mongoose.</span>document (obj, fields, skipId)](#apidoc.element.mongoose.document)
- description and source-code
```javascript
function Document(obj, fields, skipId) {
  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  var schema = this.schema;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = schema.options && schema.options.strict;
    this.$__.selected = fields;
  }

  var required = schema.requiredPaths(true);
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (obj) {
    if (obj instanceof Document) {
      this.isNew = obj.isNew;
    }
    // Skip set hooks
    if (this.$__original_set) {
      this.$__original_set(obj, undefined, true);
    } else {
      this.set(obj, undefined, true);
    }
  }

  if (!schema.options.strict && obj) {
    var _this = this,
        keys = Object.keys(this._doc);

    keys.forEach(function(key) {
      if (!(key in schema.tree)) {
        defineKey(key, null, _this);
      }
    });
  }

  applyQueue(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.error"></a>[function <span class="apidocSignatureSpan">mongoose.</span>error (msg)](#apidoc.element.mongoose.error)
- description and source-code
```javascript
function MongooseError(msg) {
  Error.call(this);
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.message = msg;
  this.name = 'MongooseError';
}
```
- example usage
```shell
...
if (!rgxProtocol.test(host)) {
  host = 'mongodb://' + host;
}

try {
  parsed = muri(host);
} catch (err) {
  this.error(err, callback);
  return new Promise.ES6(function(resolve, reject) {
    reject(err);
  });
}

database = parsed.db;
host = parsed.hosts[0].host || parsed.hosts[0].ipc;
...
```

#### <a name="apidoc.element.mongoose.model"></a>[function <span class="apidocSignatureSpan">mongoose.</span>model (doc, fields, skipId)](#apidoc.element.mongoose.model)
- description and source-code
```javascript
function Model(doc, fields, skipId) {
  Document.call(this, doc, fields, skipId, true);
}
```
- example usage
```shell
...
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model

Once we define a model through 'mongoose.model('ModelName', mySchema)', we can access it through the same function

'''js
var myModel = mongoose.model('ModelName');
'''

Or just do it all at once
...
```

#### <a name="apidoc.element.mongoose.promise"></a>[function <span class="apidocSignatureSpan">mongoose.</span>promise (fn)](#apidoc.element.mongoose.promise)
- description and source-code
```javascript
function Promise(fn) {
  MPromise.call(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query"></a>[function <span class="apidocSignatureSpan">mongoose.</span>query (conditions, options, model, collection)](#apidoc.element.mongoose.query)
- description and source-code
```javascript
function Query(conditions, options, model, collection) {
  // this stuff is for dealing with custom queries created by #toConstructor
  if (!this._mongooseOptions) {
    this._mongooseOptions = {};
  }

  // this is the case where we have a CustomQuery, we need to check if we got
  // options passed in, and if we did, merge them in
  if (options) {
    var keys = Object.keys(options);
    for (var i = 0; i < keys.length; ++i) {
      var k = keys[i];
      this._mongooseOptions[k] = options[k];
    }
  }

  if (collection) {
    this.mongooseCollection = collection;
  }

  if (model) {
    this.model = model;
    this.schema = model.schema;
  }

  // this is needed because map reduce returns a model that can be queried, but
  // all of the queries on said model should be lean
  if (this.model && this.model._mapreduce) {
    this.lean();
  }

  // inherit mquery
  mquery.call(this, this.mongooseCollection, options);

  if (conditions) {
    this.find(conditions);
  }

  if (this.schema) {
    var kareemOptions = {
      useErrorHandlers: true,
      numCallbackParams: 1
    };
    this._count = this.model.hooks.createWrapper('count',
        Query.prototype._count, this, kareemOptions);
    this._execUpdate = this.model.hooks.createWrapper('update',
        Query.prototype._execUpdate, this, kareemOptions);
    this._find = this.model.hooks.createWrapper('find',
        Query.prototype._find, this, kareemOptions);
    this._findOne = this.model.hooks.createWrapper('findOne',
        Query.prototype._findOne, this, kareemOptions);
    this._findOneAndRemove = this.model.hooks.createWrapper('findOneAndRemove',
        Query.prototype._findOneAndRemove, this, kareemOptions);
    this._findOneAndUpdate = this.model.hooks.createWrapper('findOneAndUpdate',
        Query.prototype._findOneAndUpdate, this, kareemOptions);
    this._replaceOne = this.model.hooks.createWrapper('replaceOne',
        Query.prototype._replaceOne, this, kareemOptions);
    this._updateMany = this.model.hooks.createWrapper('updateMany',
        Query.prototype._updateMany, this, kareemOptions);
    this._updateOne = this.model.hooks.createWrapper('updateOne',
        Query.prototype._updateOne, this, kareemOptions);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querycursor"></a>[function <span class="apidocSignatureSpan">mongoose.</span>querycursor (query, options)](#apidoc.element.mongoose.querycursor)
- description and source-code
```javascript
function QueryCursor(query, options) {
  Readable.call(this, { objectMode: true });

  this.cursor = null;
  this.query = query;
  this._transforms = options.transform ? [options.transform] : [];
  var _this = this;
  var model = query.model;
  model.collection.find(query._conditions, options, function(err, cursor) {
    if (_this._error) {
      cursor.close(function() {});
      _this.listeners('error').length > 0 && _this.emit('error', _this._error);
    }
    if (err) {
      return _this.emit('error', err);
    }
    _this.cursor = cursor;
    _this.emit('cursor', cursor);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querystream"></a>[function <span class="apidocSignatureSpan">mongoose.</span>querystream (query, options)](#apidoc.element.mongoose.querystream)
- description and source-code
```javascript
function QueryStream(query, options) {
  Stream.call(this);

  this.query = query;
  this.readable = true;
  this.paused = false;
  this._cursor = null;
  this._destroyed = null;
  this._fields = null;
  this._buffer = null;
  this._inline = T_INIT;
  this._running = false;
  this._transform = options && typeof options.transform === 'function'
      ? options.transform
      : K;

  // give time to hook up events
  var _this = this;
  process.nextTick(function() {
    _this._init();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema"></a>[function <span class="apidocSignatureSpan">mongoose.</span>schema (obj, options)](#apidoc.element.mongoose.schema)
- description and source-code
```javascript
function Schema(obj, options) {
  if (!(this instanceof Schema)) {
    return new Schema(obj, options);
  }

  this.obj = obj;
  this.paths = {};
  this.subpaths = {};
  this.virtuals = {};
  this.singleNestedPaths = {};
  this.nested = {};
  this.inherits = {};
  this.callQueue = [];
  this._indexes = [];
  this.methods = {};
  this.statics = {};
  this.tree = {};
  this.query = {};
  this.childSchemas = [];

  this.s = {
    hooks: new Kareem(),
    kareemHooks: IS_KAREEM_HOOK
  };

  this.options = this.defaultOptions(options);

  // build paths
  if (obj) {
    this.add(obj);
  }

  // check if _id's value is a subdocument (gh-2276)
  var _idSubDoc = obj && obj._id && utils.isObject(obj._id);

  // ensure the documents get an auto _id unless disabled
  var auto_id = !this.paths['_id'] &&
      (!this.options.noId && this.options._id) && !_idSubDoc;

  if (auto_id) {
    obj = {_id: {auto: true}};
    obj._id[this.options.typeKey] = Schema.ObjectId;
    this.add(obj);
  }

  // ensure the documents receive an id getter unless disabled
  var autoid = !this.paths['id'] &&
      (!this.options.noVirtualId && this.options.id);
  if (autoid) {
    this.virtual('id').get(idGetter);
  }

  for (var i = 0; i < this._defaultMiddleware.length; ++i) {
    var m = this._defaultMiddleware[i];
    this[m.kind](m.hook, !!m.isAsync, m.fn);
  }

  if (this.options.timestamps) {
    this.setupTimestamp(this.options.timestamps);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schematype"></a>[function <span class="apidocSignatureSpan">mongoose.</span>schematype (path, options, instance)](#apidoc.element.mongoose.schematype)
- description and source-code
```javascript
function SchemaType(path, options, instance) {
  this.path = path;
  this.instance = instance;
  this.validators = [];
  this.setters = [];
  this.getters = [];
  this.options = options;
  this._index = null;
  this.selected;

  for (var i in options) {
    if (this[i] && typeof this[i] === 'function') {
      // { unique: true, index: true }
      if (i === 'index' && this._index) {
        continue;
      }

      var opts = Array.isArray(options[i])
          ? options[i]
          : [options[i]];

      this[i].apply(this, opts);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.statemachine"></a>[function <span class="apidocSignatureSpan">mongoose.</span>statemachine ()](#apidoc.element.mongoose.statemachine)
- description and source-code
```javascript
function StateMachine() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.virtualtype"></a>[function <span class="apidocSignatureSpan">mongoose.</span>virtualtype (options, name)](#apidoc.element.mongoose.virtualtype)
- description and source-code
```javascript
function VirtualType(options, name) {
  this.path = name;
  this.getters = [];
  this.setters = [];
  this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.ES6Promise"></a>[module mongoose.ES6Promise](#apidoc.module.mongoose.ES6Promise)

#### <a name="apidoc.element.mongoose.ES6Promise.ES6Promise"></a>[function <span class="apidocSignatureSpan">mongoose.</span>ES6Promise ()](#apidoc.element.mongoose.ES6Promise.ES6Promise)
- description and source-code
```javascript
function ES6Promise() {
  throw new Error('Can\'t use ES6 promise with mpromise style constructor');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.ES6Promise.use"></a>[function <span class="apidocSignatureSpan">mongoose.ES6Promise.</span>use (Promise)](#apidoc.element.mongoose.ES6Promise.use)
- description and source-code
```javascript
use = function (Promise) {
  ES6Promise.ES6 = Promise;
}
```
- example usage
```shell
...
*/

Promise.set = function(lib) {
 if (lib === MPromise) {
   return Promise.reset();
 }
 Promise._promise = require('./ES6Promise');
 Promise._promise.use(lib);
 require('mquery').Promise = Promise._promise.ES6;
};

/**
* Resets to using mpromise
*
* @api private
...
```



# <a name="apidoc.module.mongoose.aggregate"></a>[module mongoose.aggregate](#apidoc.module.mongoose.aggregate)

#### <a name="apidoc.element.mongoose.aggregate.aggregate"></a>[function <span class="apidocSignatureSpan">mongoose.</span>aggregate ()](#apidoc.element.mongoose.aggregate.aggregate)
- description and source-code
```javascript
function Aggregate() {
  this._pipeline = [];
  this._model = undefined;
  this.options = undefined;

  if (arguments.length === 1 && util.isArray(arguments[0])) {
    this.append.apply(this, arguments[0]);
  } else {
    this.append.apply(this, arguments);
  }
}
```
- example usage
```shell
...
* ####Example:
*
*     new Aggregate();
*     new Aggregate({ $project: { a: 1, b: 1 } });
*     new Aggregate({ $project: { a: 1, b: 1 } }, { $skip: 5 });
*     new Aggregate([{ $project: { a: 1, b: 1 } }, { $skip: 5 }]);
*
* Returned when calling Model.aggregate().
*
* ####Example:
*
*     Model
*     .aggregate({ $match: { age: { $gte: 21 }}})
*     .unwind('tags')
*     .exec(callback)
...
```



# <a name="apidoc.module.mongoose.aggregate.prototype"></a>[module mongoose.aggregate.prototype](#apidoc.module.mongoose.aggregate.prototype)

#### <a name="apidoc.element.mongoose.aggregate.prototype.addCursorFlag"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>addCursorFlag (flag, value)](#apidoc.element.mongoose.aggregate.prototype.addCursorFlag)
- description and source-code
```javascript
addCursorFlag = function (flag, value) {
  if (!this.options) {
    this.options = {};
  }
  this.options[flag] = value;
  return this;
}
```
- example usage
```shell
...
};

/**
 * Adds a [cursor flag](http://mongodb.github.io/node-mongodb-native/2.1/api/Cursor.html#addCursorFlag)
 *
 * ####Example:
 *
 *     Model.aggregate(..).addCursorFlag('noCursorTimeout', true).exec();
 *
 * @param {String} flag
 * @param {Boolean} value
 * @see mongodb http://mongodb.github.io/node-mongodb-native/2.1/api/Cursor.html#addCursorFlag
 */

Aggregate.prototype.addCursorFlag = function(flag, value) {
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.allowDiskUse"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>allowDiskUse (value)](#apidoc.element.mongoose.aggregate.prototype.allowDiskUse)
- description and source-code
```javascript
allowDiskUse = function (value) {
  if (!this.options) {
    this.options = {};
  }
  this.options.allowDiskUse = value;
  return this;
}
```
- example usage
```shell
...
};

/**
 * Sets the allowDiskUse option for the aggregation query (ignored for < 2.6.0)
 *
 * ####Example:
 *
 *     Model.aggregate(..).allowDiskUse(true).exec(callback)
 *
 * @param {Boolean} value Should tell server it can use hard drive to store data during aggregation.
 * @param {Array} [tags] optional tags for this query
 * @see mongodb http://docs.mongodb.org/manual/reference/command/aggregate/
 */

Aggregate.prototype.allowDiskUse = function(value) {
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.append"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>append ()](#apidoc.element.mongoose.aggregate.prototype.append)
- description and source-code
```javascript
append = function () {
  var args = (arguments.length === 1 && util.isArray(arguments[0]))
      ? arguments[0]
      : utils.args(arguments);

  if (!args.every(isOperator)) {
    throw new Error('Arguments must be aggregate pipeline operators');
  }

  this._pipeline = this._pipeline.concat(args);

  return this;
}
```
- example usage
```shell
...
};

/**
* Appends new operators to this aggregate pipeline
*
* ####Examples:
*
*     aggregate.append({ $project: { field: 1 }}, { $limit: 2 });
*
*     // or pass an array
*     var pipeline = [{ $match: { daw: 'Logic Audio X' }} ];
*     aggregate.append(pipeline);
*
* @param {Object} ops operator(s) to append
* @return {Aggregate}
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.collation"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>collation (collation)](#apidoc.element.mongoose.aggregate.prototype.collation)
- description and source-code
```javascript
collation = function (collation) {
  if (!this.options) {
    this.options = {};
  }
  this.options.collation = collation;
  return this;
}
```
- example usage
```shell
...
};

/**
 * Adds a collation
 *
 * ####Example:
 *
 *     Model.aggregate(..).collation({ locale: 'en_US', strength: 1 }).exec();
 *
 * @param {Object} collation options
 * @param {Boolean} value
 * @see mongodb http://mongodb.github.io/node-mongodb-native/2.2/api/Collection.html#aggregate
 */

Aggregate.prototype.collation = function(collation) {
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.cursor"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>cursor (options)](#apidoc.element.mongoose.aggregate.prototype.cursor)
- description and source-code
```javascript
cursor = function (options) {
  if (!this.options) {
    this.options = {};
  }
  this.options.cursor = options || {};
  return this;
}
```
- example usage
```shell
...
/**
* Sets the cursor option option for the aggregation query (ignored for < 2.6.0).
* Note the different syntax below: .exec() returns a cursor object, and no callback
* is necessary.
*
* ####Example:
*
*     var cursor = Model.aggregate(..).cursor({ batchSize: 1000 }).exec();
*     cursor.each(function(error, doc) {
*       // use doc
*     });
*
* @param {Object} options set the cursor batch size
* @see mongodb http://mongodb.github.io/node-mongodb-native/2.0/api/AggregationCursor.html
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.exec"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>exec (callback)](#apidoc.element.mongoose.aggregate.prototype.exec)
- description and source-code
```javascript
exec = function (callback) {
  if (!this._model) {
    throw new Error('Aggregate not bound to any Model');
  }
  var _this = this;
  var Promise = PromiseProvider.get();
  var options = utils.clone(this.options);

  if (options && options.cursor) {
    if (options.cursor.async) {
      delete options.cursor.async;
      return new Promise.ES6(function(resolve) {
        if (!_this._model.collection.buffer) {
          process.nextTick(function() {
            var cursor = _this._model.collection.
              aggregate(_this._pipeline, options || {});
            decorateCursor(cursor);
            resolve(cursor);
            callback && callback(null, cursor);
          });
          return;
        }
        _this._model.collection.emitter.once('queue', function() {
          var cursor = _this._model.collection.
            aggregate(_this._pipeline, options || {});
          decorateCursor(cursor);
          resolve(cursor);
          callback && callback(null, cursor);
        });
      });
    }
    var cursor = this._model.collection.
      aggregate(this._pipeline, this.options || {});
    decorateCursor(cursor);
    return cursor;
  }

  return new Promise.ES6(function(resolve, reject) {
    if (!_this._pipeline.length) {
      var err = new Error('Aggregate has empty pipeline');
      if (callback) {
        callback(err);
      }
      reject(err);
      return;
    }

    prepareDiscriminatorPipeline(_this);

    _this._model
        .collection
        .aggregate(_this._pipeline, _this.options || {}, function(error, result) {
          if (error) {
            if (callback) {
              callback(error);
            }
            reject(error);
            return;
          }

          if (callback) {
            callback(null, result);
          }
          resolve(result);
        });
  });
}
```
- example usage
```shell
...

/**
* ES6 Promise wrapper constructor.
*
* Promises are returned from executed queries. Example:
*
*     var query = Candy.find({ bar: true });
*     var promise = query.exec();
*
* DEPRECATED. Mongoose 5.0 will use native promises by default (or bluebird,
* if native promises are not present) but still
* support plugging in your own ES6-compatible promises library. Mongoose 5.0
* will **not** support mpromise.
*
* @param {Function} fn a function which will be called when the promise is resolved that accepts 'fn(err, ...){}' as signature
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.explain"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>explain (callback)](#apidoc.element.mongoose.aggregate.prototype.explain)
- description and source-code
```javascript
explain = function (callback) {
  var _this = this;
  var Promise = PromiseProvider.get();
  return new Promise.ES6(function(resolve, reject) {
    if (!_this._pipeline.length) {
      var err = new Error('Aggregate has empty pipeline');
      if (callback) {
        callback(err);
      }
      reject(err);
      return;
    }

    prepareDiscriminatorPipeline(_this);

    _this._model
        .collection
        .aggregate(_this._pipeline, _this.options || {})
        .explain(function(error, result) {
          if (error) {
            if (callback) {
              callback(error);
            }
            reject(error);
            return;
          }

          if (callback) {
            callback(null, result);
          }
          resolve(result);
        });
  });
}
```
- example usage
```shell
...
};

/**
 * Execute the aggregation with explain
 *
 * ####Example:
 *
 *     Model.aggregate(..).explain(callback)
 *
 * @param {Function} callback
 * @return {Promise}
 */

Aggregate.prototype.explain = function(callback) {
var _this = this;
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.facet"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>facet (options)](#apidoc.element.mongoose.aggregate.prototype.facet)
- description and source-code
```javascript
facet = function (options) {
  return this.append({$facet: options});
}
```
- example usage
```shell
...
};

/**
* Combines multiple aggregation pipelines.
*
* ####Example:
*     Model.aggregate(...)
*      .facet({
*        books: [{ groupBy: '$author' }],
*        price: [{ $bucketAuto: { groupBy: '$price', buckets: 2 } }]
*      })
*      .exec();
*
*     // Output: { books: [...], price: [{...}, {...}] }
*
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.graphLookup"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>graphLookup (options)](#apidoc.element.mongoose.aggregate.prototype.graphLookup)
- description and source-code
```javascript
graphLookup = function (options) {
  var cloneOptions = {};
  if (options) {
    if (!utils.isObject(options)) {
      throw new TypeError('Invalid graphLookup() argument. Must be an object.');
    }

    utils.mergeClone(cloneOptions, options);
    var startWith = cloneOptions.startWith;

    if (startWith && typeof startWith === 'string') {
      cloneOptions.startWith = cloneOptions.startWith.charAt(0) === '$' ?
        cloneOptions.startWith :
        '$' + cloneOptions.startWith;
    }

  }
  return this.append({ $graphLookup: cloneOptions });
}
```
- example usage
```shell
...
/**
* Appends new custom $graphLookup operator(s) to this aggregate pipeline, performing a recursive search on a collection.
*
* Note that graphLookup can only consume at most 100MB of memory, and does not allow disk use even if '{ allowDiskUse: true }' is
 specified.
*
* #### Examples:
*      // Suppose we have a collection of courses, where a document might look like '{ _id: 0, name: 'Calculus', prerequisite: '
Trigonometry'}' and '{ _id: 0, name: 'Trigonometry', prerequisite: 'Algebra' }'
*      aggregate.graphLookup({ from: 'courses', startWith: '$prerequisite', connectFromField: 'prerequisite', connectToField: 'name
', as: 'prerequisites', maxDepth: 3 }) // this will recursively search the 'courses' collection up to 3 prerequisites
*
* @see $graphLookup https://docs.mongodb.com/manual/reference/operator/aggregation/graphLookup/#pipe._S_graphLookup
* @param {Object} options to $graphLookup as described in the above link
* @return {Aggregate}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.group"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>group (arg)](#apidoc.element.mongoose.aggregate.prototype.group)
- description and source-code
```javascript
group = function (arg) {
  var op = {};
  op['$' + $operator] = arg;
  return this.append(op);
}
```
- example usage
```shell
...
};

/**
* Appends a new custom $group operator to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.group({ _id: "$department" });
*
* @see $group http://docs.mongodb.org/manual/reference/aggregation/group/
* @method group
* @memberOf Aggregate
* @param {Object} arg $group operator contents
* @return {Aggregate}
* @api public
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.limit"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>limit (arg)](#apidoc.element.mongoose.aggregate.prototype.limit)
- description and source-code
```javascript
limit = function (arg) {
  var op = {};
  op['$' + $operator] = arg;
  return this.append(op);
}
```
- example usage
```shell
...
*/

/**
* Appends a new $limit operator to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.limit(10);
*
* @see $limit http://docs.mongodb.org/manual/reference/aggregation/limit/
* @method limit
* @memberOf Aggregate
* @param {Number} num maximum number of records to pass to the next stage
* @return {Aggregate}
* @api public
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.lookup"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>lookup (options)](#apidoc.element.mongoose.aggregate.prototype.lookup)
- description and source-code
```javascript
lookup = function (options) {
  return this.append({$lookup: options});
}
```
- example usage
```shell
...
};

/**
* Appends new custom $lookup operator(s) to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.lookup({ from: 'users', localField: 'userId', foreignField: '_id', as: 'users' });
*
* @see $lookup https://docs.mongodb.org/manual/reference/operator/aggregation/lookup/#pipe._S_lookup
* @param {Object} options to $lookup as described in the above link
* @return {Aggregate}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.match"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>match (arg)](#apidoc.element.mongoose.aggregate.prototype.match)
- description and source-code
```javascript
match = function (arg) {
  var op = {};
  op['$' + $operator] = arg;
  return this.append(op);
}
```
- example usage
```shell
...
*/

/**
* Appends a new custom $match operator to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.match({ department: { $in: [ "sales", "engineering" } } });
*
* @see $match http://docs.mongodb.org/manual/reference/aggregation/match/
* @method match
* @memberOf Aggregate
* @param {Object} arg $match operator contents
* @return {Aggregate}
* @api public
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.model"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>model (model)](#apidoc.element.mongoose.aggregate.prototype.model)
- description and source-code
```javascript
model = function (model) {
  this._model = model;
  return this;
}
```
- example usage
```shell
...
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model

Once we define a model through 'mongoose.model('ModelName', mySchema)', we can access it through the same function

'''js
var myModel = mongoose.model('ModelName');
'''

Or just do it all at once
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.near"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>near (arg)](#apidoc.element.mongoose.aggregate.prototype.near)
- description and source-code
```javascript
near = function (arg) {
  var op = {};
  op.$geoNear = arg;
  return this.append(op);
}
```
- example usage
```shell
...
*
* ####NOTE:
*
* **MUST** be used as the first operator in the pipeline.
*
* ####Examples:
*
*     aggregate.near({
*       near: [40.724, -73.997],
*       distanceField: "dist.calculated", // required
*       maxDistance: 0.008,
*       query: { type: "public" },
*       includeLocs: "dist.location",
*       uniqueDocs: true,
*       num: 5
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.out"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>out (arg)](#apidoc.element.mongoose.aggregate.prototype.out)
- description and source-code
```javascript
out = function (arg) {
  var op = {};
  op['$' + $operator] = arg;
  return this.append(op);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.project"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>project (arg)](#apidoc.element.mongoose.aggregate.prototype.project)
- description and source-code
```javascript
project = function (arg) {
  var fields = {};

  if (typeof arg === 'object' && !util.isArray(arg)) {
    Object.keys(arg).forEach(function(field) {
      fields[field] = arg[field];
    });
  } else if (arguments.length === 1 && typeof arg === 'string') {
    arg.split(/\s+/).forEach(function(field) {
      if (!field) {
        return;
      }
      var include = field[0] === '-' ? 0 : 1;
      if (include === 0) {
        field = field.substring(1);
      }
      fields[field] = include;
    });
  } else {
    throw new Error('Invalid project() argument. Must be string or object');
  }

  return this.append({$project: fields});
}
```
- example usage
```shell
...
* Appends a new $project operator to this aggregate pipeline.
*
* Mongoose query [selection syntax](#query_Query-select) is also supported.
*
* ####Examples:
*
*     // include a, include b, exclude _id
*     aggregate.project("a b -_id");
*
*     // or you may use object notation, useful when
*     // you have keys already prefixed with a "-"
*     aggregate.project({a: 1, b: 1, _id: 0});
*
*     // reshaping documents
*     aggregate.project({
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.read"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>read (pref, tags)](#apidoc.element.mongoose.aggregate.prototype.read)
- description and source-code
```javascript
read = function (pref, tags) {
  if (!this.options) {
    this.options = {};
  }
  read.call(this, pref, tags);
  return this;
}
```
- example usage
```shell
...
};

/**
* Sets the readPreference option for the aggregation query.
*
* ####Example:
*
*     Model.aggregate(..).read('primaryPreferred').exec(callback)
*
* @param {String} pref one of the listed preference options or their aliases
* @param {Array} [tags] optional tags for this query
* @see mongodb http://docs.mongodb.org/manual/applications/replication/#read-preference
* @see driver http://mongodb.github.com/node-mongodb-native/driver-articles/anintroductionto1_1and2_2.html#read-preferences
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.sample"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>sample (size)](#apidoc.element.mongoose.aggregate.prototype.sample)
- description and source-code
```javascript
sample = function (size) {
  return this.append({$sample: {size: size}});
}
```
- example usage
```shell
...
};

/**
* Appepnds new custom $sample operator(s) to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.sample(3); // Add a pipeline that picks 3 random documents
*
* @see $sample https://docs.mongodb.org/manual/reference/operator/aggregation/sample/#pipe._S_sample
* @param {Number} size number of random documents to pick
* @return {Aggregate}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.skip"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>skip (arg)](#apidoc.element.mongoose.aggregate.prototype.skip)
- description and source-code
```javascript
skip = function (arg) {
  var op = {};
  op['$' + $operator] = arg;
  return this.append(op);
}
```
- example usage
```shell
...
*/

/**
* Appends a new $skip operator to this aggregate pipeline.
*
* ####Examples:
*
*     aggregate.skip(10);
*
* @see $skip http://docs.mongodb.org/manual/reference/aggregation/skip/
* @method skip
* @memberOf Aggregate
* @param {Number} num number of records to skip before next stage
* @return {Aggregate}
* @api public
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.sort"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>sort (arg)](#apidoc.element.mongoose.aggregate.prototype.sort)
- description and source-code
```javascript
sort = function (arg) {
  // TODO refactor to reuse the query builder logic

  var sort = {};

  if (arg.constructor.name === 'Object') {
    var desc = ['desc', 'descending', -1];
    Object.keys(arg).forEach(function(field) {
      sort[field] = desc.indexOf(arg[field]) === -1 ? 1 : -1;
    });
  } else if (arguments.length === 1 && typeof arg === 'string') {
    arg.split(/\s+/).forEach(function(field) {
      if (!field) {
        return;
      }
      var ascend = field[0] === '-' ? -1 : 1;
      if (ascend === -1) {
        field = field.substring(1);
      }
      sort[field] = ascend;
    });
  } else {
    throw new TypeError('Invalid sort() argument. Must be a string or object.');
  }

  return this.append({$sort: sort});
}
```
- example usage
```shell
...
* If an object is passed, values allowed are 'asc', 'desc', 'ascending', 'descending', '1', and '-1'.
*
* If a string is passed, it must be a space delimited list of path names. The sort order of each path is ascending unless the path
 name is prefixed with '-' which will be treated as descending.
*
* ####Examples:
*
*     // these are equivalent
*     aggregate.sort({ field: 'asc', test: -1 });
*     aggregate.sort('field -test');
*
* @see $sort http://docs.mongodb.org/manual/reference/aggregation/sort/
* @param {Object|String} arg
* @return {Aggregate} this
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.then"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>then (resolve, reject)](#apidoc.element.mongoose.aggregate.prototype.then)
- description and source-code
```javascript
then = function (resolve, reject) {
  return this.exec().then(resolve, reject);
}
```
- example usage
```shell
...
*
* ####Example:
*
*     aggregate.exec(callback);
*
*     // Because a promise is returned, the 'callback' is optional.
*     var promise = aggregate.exec();
*     promise.then(..);
*
* @see Promise #promise_Promise
* @param {Function} [callback]
* @return {Promise}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.aggregate.prototype.unwind"></a>[function <span class="apidocSignatureSpan">mongoose.aggregate.prototype.</span>unwind ()](#apidoc.element.mongoose.aggregate.prototype.unwind)
- description and source-code
```javascript
unwind = function () {
  var args = utils.args(arguments);

  var res = [];
  for (var i = 0; i < args.length; ++i) {
    var arg = args[i];
    if (arg && typeof arg === 'object') {
      res.push({ $unwind: arg });
    } else if (typeof arg === 'string') {
      res.push({
        $unwind: (arg && arg.charAt(0) === '$') ? arg : '$' + arg
      });
    } else {
      throw new Error('Invalid arg "' + arg + '" to unwind(), ' +
        'must be string or object');
    }
  }

  return this.append.apply(this, res);
}
```
- example usage
```shell
...
*
* Returned when calling Model.aggregate().
*
* ####Example:
*
*     Model
*     .aggregate({ $match: { age: { $gte: 21 }}})
*     .unwind('tags')
*     .exec(callback)
*
* ####Note:
*
* - The documents returned are plain javascript objects, not mongoose documents (since any shape of document can be returned).
* - Requires MongoDB >= 2.1
* - Mongoose does **not** cast pipeline stages. 'new Aggregate({ $match: { _id: '00000000000000000000000a' } });' will not work
unless '_id' is a string in the database. Use 'new Aggregate({ $match: { _id: mongoose.Types.ObjectId('00000000000000000000000a') } });'
instead.
...
```



# <a name="apidoc.module.mongoose.browser"></a>[module mongoose.browser](#apidoc.module.mongoose.browser)

#### <a name="apidoc.element.mongoose.browser.Document"></a>[function <span class="apidocSignatureSpan">mongoose.browser.</span>Document (obj, fields, skipId)](#apidoc.element.mongoose.browser.Document)
- description and source-code
```javascript
function Document(obj, fields, skipId) {
  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  var schema = this.schema;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = schema.options && schema.options.strict;
    this.$__.selected = fields;
  }

  var required = schema.requiredPaths(true);
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (obj) {
    if (obj instanceof Document) {
      this.isNew = obj.isNew;
    }
    // Skip set hooks
    if (this.$__original_set) {
      this.$__original_set(obj, undefined, true);
    } else {
      this.set(obj, undefined, true);
    }
  }

  if (!schema.options.strict && obj) {
    var _this = this,
        keys = Object.keys(this._doc);

    keys.forEach(function(key) {
      if (!(key in schema.tree)) {
        defineKey(key, null, _this);
      }
    });
  }

  applyQueue(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browser.Error"></a>[function <span class="apidocSignatureSpan">mongoose.browser.</span>Error (msg)](#apidoc.element.mongoose.browser.Error)
- description and source-code
```javascript
function MongooseError(msg) {
  Error.call(this);
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.message = msg;
  this.name = 'MongooseError';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browser.Schema"></a>[function <span class="apidocSignatureSpan">mongoose.browser.</span>Schema (obj, options)](#apidoc.element.mongoose.browser.Schema)
- description and source-code
```javascript
function Schema(obj, options) {
  if (!(this instanceof Schema)) {
    return new Schema(obj, options);
  }

  this.obj = obj;
  this.paths = {};
  this.subpaths = {};
  this.virtuals = {};
  this.singleNestedPaths = {};
  this.nested = {};
  this.inherits = {};
  this.callQueue = [];
  this._indexes = [];
  this.methods = {};
  this.statics = {};
  this.tree = {};
  this.query = {};
  this.childSchemas = [];

  this.s = {
    hooks: new Kareem(),
    kareemHooks: IS_KAREEM_HOOK
  };

  this.options = this.defaultOptions(options);

  // build paths
  if (obj) {
    this.add(obj);
  }

  // check if _id's value is a subdocument (gh-2276)
  var _idSubDoc = obj && obj._id && utils.isObject(obj._id);

  // ensure the documents get an auto _id unless disabled
  var auto_id = !this.paths['_id'] &&
      (!this.options.noId && this.options._id) && !_idSubDoc;

  if (auto_id) {
    obj = {_id: {auto: true}};
    obj._id[this.options.typeKey] = Schema.ObjectId;
    this.add(obj);
  }

  // ensure the documents receive an id getter unless disabled
  var autoid = !this.paths['id'] &&
      (!this.options.noVirtualId && this.options.id);
  if (autoid) {
    this.virtual('id').get(idGetter);
  }

  for (var i = 0; i < this._defaultMiddleware.length; ++i) {
    var m = this._defaultMiddleware[i];
    this[m.kind](m.hook, !!m.isAsync, m.fn);
  }

  if (this.options.timestamps) {
    this.setupTimestamp(this.options.timestamps);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browser.SchemaType"></a>[function <span class="apidocSignatureSpan">mongoose.browser.</span>SchemaType (path, options, instance)](#apidoc.element.mongoose.browser.SchemaType)
- description and source-code
```javascript
function SchemaType(path, options, instance) {
  this.path = path;
  this.instance = instance;
  this.validators = [];
  this.setters = [];
  this.getters = [];
  this.options = options;
  this._index = null;
  this.selected;

  for (var i in options) {
    if (this[i] && typeof this[i] === 'function') {
      // { unique: true, index: true }
      if (i === 'index' && this._index) {
        continue;
      }

      var opts = Array.isArray(options[i])
          ? options[i]
          : [options[i]];

      this[i].apply(this, opts);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browser.VirtualType"></a>[function <span class="apidocSignatureSpan">mongoose.browser.</span>VirtualType (options, name)](#apidoc.element.mongoose.browser.VirtualType)
- description and source-code
```javascript
function VirtualType(options, name) {
  this.path = name;
  this.getters = [];
  this.setters = [];
  this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.browserDocument"></a>[module mongoose.browserDocument](#apidoc.module.mongoose.browserDocument)

#### <a name="apidoc.element.mongoose.browserDocument.browserDocument"></a>[function <span class="apidocSignatureSpan">mongoose.</span>browserDocument (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument.browserDocument)
- description and source-code
```javascript
function Document(obj, schema, fields, skipId, skipInit) {
  if (!(this instanceof Document)) {
    return new Document(obj, schema, fields, skipId, skipInit);
  }


  if (utils.isObject(schema) && !schema.instanceOfSchema) {
    schema = new Schema(schema);
  }

  // When creating EmbeddedDocument, it already has the schema and he doesn't need the _id
  schema = this.schema || schema;

  // Generate ObjectId if it is missing, but it requires a scheme
  if (!this.schema && schema.options._id) {
    obj = obj || {};

    if (obj._id === undefined) {
      obj._id = new ObjectId();
    }
  }

  if (!schema) {
    throw new MongooseError.MissingSchemaError();
  }

  this.$__setSchema(schema);

  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = this.schema.options && this.schema.options.strict;
    this.$__.selected = fields;
  }

  var required = this.schema.requiredPaths();
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (!skipInit && obj) {
    this.init(obj);
  }

  this.$__registerHooksFromSchema();

  // apply methods
  for (var m in schema.methods) {
    this[m] = schema.methods[m];
  }
  // apply statics
  for (var s in schema.statics) {
    this[s] = schema.statics[s];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browserDocument.ValidationError"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>ValidationError (instance)](#apidoc.element.mongoose.browserDocument.ValidationError)
- description and source-code
```javascript
function ValidationError(instance) {
  this.errors = {};
  if (instance && instance.constructor.name === 'model') {
    MongooseError.call(this, instance.constructor.modelName + ' validation failed');
  } else {
    MongooseError.call(this, 'Validation failed');
  }
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.name = 'ValidationError';
  if (instance) {
    instance.errors = this.errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browserDocument.addListener"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>addListener ()](#apidoc.element.mongoose.browserDocument.addListener)
- description and source-code
```javascript
addListener = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browserDocument.emit"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>emit ()](#apidoc.element.mongoose.browserDocument.emit)
- description and source-code
```javascript
emit = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
...
You can intercept method arguments via middleware.

For example, this would allow you to broadcast changes about your Documents every time someone 'set's a path in your Document to
 a new value:

'''js
schema.pre('set', function (next, path, val, typel) {
  // 'this' is the current Document
  this.emit('set', path, val);

  // Pass control to the next pre
  next();
});
'''

Moreover, you can mutate the incoming 'method' arguments so that subsequent middleware see different values for those arguments.
To do so, just pass the new values to 'next':
...
```

#### <a name="apidoc.element.mongoose.browserDocument.listeners"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>listeners ()](#apidoc.element.mongoose.browserDocument.listeners)
- description and source-code
```javascript
listeners = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
...
      doc[pair[0]].apply(doc, pair[1]);
    }
  }
}

Document.prototype.$__handleReject = function handleReject(err) {
  // emit on the Model if listening
  if (this.listeners('error').length) {
    this.emit('error', err);
  } else if (this.constructor.listeners && this.constructor.listeners('error').length) {
    this.constructor.emit('error', err);
  } else if (this.listeners && this.listeners('error').length) {
    this.emit('error', err);
  }
};
...
```

#### <a name="apidoc.element.mongoose.browserDocument.on"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>on ()](#apidoc.element.mongoose.browserDocument.on)
- description and source-code
```javascript
on = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
...
 * - 2 = connecting
 * - 3 = disconnecting
 *
 * Each state change emits its associated event name.
 *
 * ####Example
 *
 *     conn.on('connected', callback);
 *     conn.on('disconnected', callback);
 *
 * @property readyState
 * @api public
 */

Object.defineProperty(Connection.prototype, 'readyState', {
...
```

#### <a name="apidoc.element.mongoose.browserDocument.once"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>once ()](#apidoc.element.mongoose.browserDocument.once)
- description and source-code
```javascript
once = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
...
        aggregate(_this._pipeline, options || {});
      decorateCursor(cursor);
      resolve(cursor);
      callback && callback(null, cursor);
    });
    return;
  }
  _this._model.collection.emitter.once('queue', function() {
    var cursor = _this._model.collection.
      aggregate(_this._pipeline, options || {});
    decorateCursor(cursor);
    resolve(cursor);
    callback && callback(null, cursor);
  });
});
...
```

#### <a name="apidoc.element.mongoose.browserDocument.removeAllListeners"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>removeAllListeners ()](#apidoc.element.mongoose.browserDocument.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browserDocument.removeListener"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>removeListener ()](#apidoc.element.mongoose.browserDocument.removeListener)
- description and source-code
```javascript
removeListener = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.browserDocument.setMaxListeners"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.</span>setMaxListeners ()](#apidoc.element.mongoose.browserDocument.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function () {
  return Document.$emitter[emitterFn].apply(Document.$emitter, arguments);
}
```
- example usage
```shell
...
}

var required = this.schema.requiredPaths();
for (var i = 0; i < required.length; ++i) {
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);

if (!skipInit && obj) {
  this.init(obj);
}

this.$__registerHooksFromSchema();
...
```



# <a name="apidoc.module.mongoose.browserDocument.prototype"></a>[module mongoose.browserDocument.prototype](#apidoc.module.mongoose.browserDocument.prototype)

#### <a name="apidoc.element.mongoose.browserDocument.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mongoose.browserDocument.prototype.</span>constructor (obj, schema, fields, skipId, skipInit)](#apidoc.element.mongoose.browserDocument.prototype.constructor)
- description and source-code
```javascript
function Document(obj, schema, fields, skipId, skipInit) {
  if (!(this instanceof Document)) {
    return new Document(obj, schema, fields, skipId, skipInit);
  }


  if (utils.isObject(schema) && !schema.instanceOfSchema) {
    schema = new Schema(schema);
  }

  // When creating EmbeddedDocument, it already has the schema and he doesn't need the _id
  schema = this.schema || schema;

  // Generate ObjectId if it is missing, but it requires a scheme
  if (!this.schema && schema.options._id) {
    obj = obj || {};

    if (obj._id === undefined) {
      obj._id = new ObjectId();
    }
  }

  if (!schema) {
    throw new MongooseError.MissingSchemaError();
  }

  this.$__setSchema(schema);

  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = this.schema.options && this.schema.options.strict;
    this.$__.selected = fields;
  }

  var required = this.schema.requiredPaths();
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (!skipInit && obj) {
    this.init(obj);
  }

  this.$__registerHooksFromSchema();

  // apply methods
  for (var m in schema.methods) {
    this[m] = schema.methods[m];
  }
  // apply statics
  for (var s in schema.statics) {
    this[s] = schema.statics[s];
  }
}
```
- example usage
```shell
...
}

if (obj.constructor) {
  switch (exports.getFunctionName(obj.constructor)) {
    case 'Object':
      return cloneObject(obj, options);
    case 'Date':
      return new obj.constructor(+obj);
    case 'RegExp':
      return cloneRegExp(obj);
    default:
      // ignore
      break;
  }
}
...
```



# <a name="apidoc.module.mongoose.collection"></a>[module mongoose.collection](#apidoc.module.mongoose.collection)

#### <a name="apidoc.element.mongoose.collection.collection"></a>[function <span class="apidocSignatureSpan">mongoose.</span>collection (name, conn, opts)](#apidoc.element.mongoose.collection.collection)
- description and source-code
```javascript
function Collection(name, conn, opts) {
  if (opts === void 0) {
    opts = {};
  }
  if (opts.capped === void 0) {
    opts.capped = {};
  }

  opts.bufferCommands = undefined === opts.bufferCommands
      ? true
      : opts.bufferCommands;

  if (typeof opts.capped === 'number') {
    opts.capped = {size: opts.capped};
  }

  this.opts = opts;
  this.name = name;
  this.collectionName = name;
  this.conn = conn;
  this.queue = [];
  this.buffer = this.opts.bufferCommands;
  this.emitter = new EventEmitter();

  if (STATES.connected === this.conn.readyState) {
    this.onOpen();
  }
}
```
- example usage
```shell
...
model.prototype.$__setSchema(schema);

var collectionOptions = {
  bufferCommands: schema.options.bufferCommands,
  capped: schema.options.capped
};

model.prototype.collection = connection.collection(
    collectionName
    , collectionOptions
);

// apply methods and statics
applyMethods(model, schema);
applyStatics(model, schema);
...
```



# <a name="apidoc.module.mongoose.collection.prototype"></a>[module mongoose.collection.prototype](#apidoc.module.mongoose.collection.prototype)

#### <a name="apidoc.element.mongoose.collection.prototype.addQueue"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>addQueue (name, args)](#apidoc.element.mongoose.collection.prototype.addQueue)
- description and source-code
```javascript
addQueue = function (name, args) {
  this.queue.push([name, args]);
  return this;
}
```
- example usage
```shell
...
      create();
    }));
  };

  setImmediate(function() {
    // If buffering is off, do this manually.
    if (options._automatic && !model.collection.collection) {
      model.collection.addQueue(create, []);
    } else {
      create();
    }
  });
}

function _handleSafe(options) {
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.doQueue"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>doQueue ()](#apidoc.element.mongoose.collection.prototype.doQueue)
- description and source-code
```javascript
doQueue = function () {
  for (var i = 0, l = this.queue.length; i < l; i++) {
    if (typeof this.queue[i][0] === 'function') {
      this.queue[i][0].apply(this, this.queue[i][1]);
    } else {
      this[this.queue[i][0]].apply(this, this.queue[i][1]);
    }
  }
  this.queue = [];
  var _this = this;
  process.nextTick(function() {
    _this.emitter.emit('queue');
  });
  return this;
}
```
- example usage
```shell
...
* Called when the database connects
*
* @api private
*/

Collection.prototype.onOpen = function() {
 this.buffer = false;
 this.doQueue();
};

/**
* Called when the database disconnects
*
* @api private
*/
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.ensureIndex"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>ensureIndex ()](#apidoc.element.mongoose.collection.prototype.ensureIndex)
- description and source-code
```javascript
ensureIndex = function () {
  throw new Error('Collection#ensureIndex unimplemented by driver');
}
```
- example usage
```shell
...

  var indexFields = index[0];
  var options = index[1];
  _handleSafe(options);

  indexSingleStart(indexFields, options);

  model.collection.ensureIndex(indexFields, options, utils.tick(function(err, name) {
    indexSingleDone(err, indexFields, options, name);
    if (err) {
      return done(err);
    }
    create();
  }));
};
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.find"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>find ()](#apidoc.element.mongoose.collection.prototype.find)
- description and source-code
```javascript
find = function () {
  throw new Error('Collection#find unimplemented by driver');
}
```
- example usage
```shell
...
  //
});
'''

Or we can find documents from the same collection

'''js
MyModel.find({}, function (err, docs) {
  // docs.forEach
});
'''

You can also 'findOne', 'findById', 'update', etc. For more details check out [the docs](http://mongoosejs.com/docs/queries.html
).

**Important!** If you opened a separate connection using 'mongoose.createConnection()' but attempt to access the model through '
mongoose.model('ModelName')' it will not work as expected since it is not hooked up to an active db connection. In this case access
 your model through the connection you created:
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.findAndModify"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>findAndModify ()](#apidoc.element.mongoose.collection.prototype.findAndModify)
- description and source-code
```javascript
findAndModify = function () {
  throw new Error('Collection#findAndModify unimplemented by driver');
}
```
- example usage
```shell
...
  };

  if (opts.runValidators && doValidate) {
var _callback = function(error) {
  if (error) {
    return callback(error);
  }
  _this._collection.findAndModify(castedQuery, castedDoc, opts, utils.tick(function(error, res) {
    return cb(error, res ? res.value : res, res);
  }));
};

try {
  doValidate(_callback);
} catch (error) {
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.findOne"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>findOne ()](#apidoc.element.mongoose.collection.prototype.findOne)
- description and source-code
```javascript
findOne = function () {
  throw new Error('Collection#findOne unimplemented by driver');
}
```
- example usage
```shell
...
};

/**
* Checks if 'path' was selected in the source query which initialized this document.
*
* ####Example
*
*     Thing.findOne().select('name').exec(function (err, doc) {
*        doc.isSelected('name') // true
*        doc.isSelected('age')  // false
*     })
*
* @param {String} path
* @return {Boolean}
* @api public
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.getIndexes"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>getIndexes ()](#apidoc.element.mongoose.collection.prototype.getIndexes)
- description and source-code
```javascript
getIndexes = function () {
  throw new Error('Collection#getIndexes unimplemented by driver');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.collection.prototype.insert"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>insert ()](#apidoc.element.mongoose.collection.prototype.insert)
- description and source-code
```javascript
insert = function () {
  throw new Error('Collection#insert unimplemented by driver');
}
```
- example usage
```shell
...
      setTimeout(function() {
callback(new Error('document must have an _id before saving'));
      }, 0);
      return;
    }

    this.$__version(true, obj);
    this.collection.insert(obj, options.safe, function(err, ret) {
      if (err) {
_this.isNew = true;
_this.emit('isNew', true);
_this.constructor.emit('isNew', true);

callback(err);
return;
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.mapReduce"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>mapReduce ()](#apidoc.element.mongoose.collection.prototype.mapReduce)
- description and source-code
```javascript
mapReduce = function () {
  throw new Error('Collection#mapReduce unimplemented by driver');
}
```
- example usage
```shell
...
* 'o' is an object specifying all mapReduce options as well as the map and reduce functions. All options are delegated to the driver
 implementation. See [node-mongodb-native mapReduce() documentation](http://mongodb.github.io/node-mongodb-native/api-generated/
collection.html#mapreduce) for more detail about options.
*
* ####Example:
*
*     var o = {};
*     o.map = function () { emit(this.name, 1) }
*     o.reduce = function (k, vals) { return vals.length }
*     User.mapReduce(o, function (err, results) {
*       console.log(results)
*     })
*
* ####Other options:
*
* - 'query' {Object} query filter object.
* - 'sort' {Object} sort input objects using this key
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.onClose"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>onClose ()](#apidoc.element.mongoose.collection.prototype.onClose)
- description and source-code
```javascript
onClose = function () {
  if (this.opts.bufferCommands) {
    this.buffer = true;
  }
}
```
- example usage
```shell
...
case 1: // connected
case 4: // unauthorized
  this.readyState = STATES.disconnecting;
  this.doClose(function(err) {
    if (err) {
      _this.error(err, callback);
    } else {
      _this.onClose();
      callback && callback();
    }
  });
  break;

case 2: // connecting
  this.once('open', function() {
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.onOpen"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>onOpen ()](#apidoc.element.mongoose.collection.prototype.onOpen)
- description and source-code
```javascript
onOpen = function () {
  this.buffer = false;
  this.doQueue();
}
```
- example usage
```shell
...
 this.collectionName = name;
 this.conn = conn;
 this.queue = [];
 this.buffer = this.opts.bufferCommands;
 this.emitter = new EventEmitter();

 if (STATES.connected === this.conn.readyState) {
   this.onOpen();
 }
}

/**
* The collection name
*
* @api public
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.save"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>save ()](#apidoc.element.mongoose.collection.prototype.save)
- description and source-code
```javascript
save = function () {
  throw new Error('Collection#save unimplemented by driver');
}
```
- example usage
```shell
...
Then Mongoose will create the model for your __tickets__ collection, not your __ticket__ collection.

Once we have our model, we can then instantiate it, and save it:

'''js
var instance = new MyModel();
instance.my.key = 'hello';
instance.save(function (err) {
  //
});
'''

Or we can find documents from the same collection

'''js
...
```

#### <a name="apidoc.element.mongoose.collection.prototype.update"></a>[function <span class="apidocSignatureSpan">mongoose.collection.prototype.</span>update ()](#apidoc.element.mongoose.collection.prototype.update)
- description and source-code
```javascript
update = function () {
  throw new Error('Collection#update unimplemented by driver');
}
```
- example usage
```shell
...
}

/**
* Sends an update command with this document '_id' as the query selector.
*
* ####Example:
*
*     weirdCar.update({$inc: {wheels:1}}, { w: 1 }, callback);
*
* ####Valid options:
*
*  - same as in [Model.update](#model_Model.update)
*
* @see Model.update #model_Model.update
* @param {Object} doc
...
```



# <a name="apidoc.module.mongoose.connection"></a>[module mongoose.connection](#apidoc.module.mongoose.connection)

#### <a name="apidoc.element.mongoose.connection.connection"></a>[function <span class="apidocSignatureSpan">mongoose.</span>connection (base)](#apidoc.element.mongoose.connection.connection)
- description and source-code
```javascript
function Connection(base) {
  this.base = base;
  this.collections = {};
  this.models = {};
  this.config = {autoIndex: true};
  this.replica = false;
  this.hosts = null;
  this.host = null;
  this.port = null;
  this.user = null;
  this.pass = null;
  this.name = null;
  this.options = null;
  this.otherDbs = [];
  this._readyState = STATES.disconnected;
  this._closeCalled = false;
  this._hasOpened = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.connection.prototype"></a>[module mongoose.connection.prototype](#apidoc.module.mongoose.connection.prototype)

#### <a name="apidoc.element.mongoose.connection.prototype._close"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>_close (callback)](#apidoc.element.mongoose.connection.prototype._close)
- description and source-code
```javascript
_close = function (callback) {
  var _this = this;
  this._closeCalled = true;

  switch (this.readyState) {
    case 0: // disconnected
      callback && callback();
      break;

    case 1: // connected
    case 4: // unauthorized
      this.readyState = STATES.disconnecting;
      this.doClose(function(err) {
        if (err) {
          _this.error(err, callback);
        } else {
          _this.onClose();
          callback && callback();
        }
      });
      break;

    case 2: // connecting
      this.once('open', function() {
        _this.close(callback);
      });
      break;

    case 3: // disconnecting
      if (!callback) {
        break;
      }
      this.once('close', function() {
        callback();
      });
      break;
  }

  return this;
}
```
- example usage
```shell
...
 * @api public
 */

Connection.prototype.close = function(callback) {
var _this = this;
var Promise = PromiseProvider.get();
return new Promise.ES6(function(resolve, reject) {
  _this._close(function(error) {
    callback && callback(error);
    if (error) {
      reject(error);
      return;
    }
    resolve();
  });
...
```

#### <a name="apidoc.element.mongoose.connection.prototype._open"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>_open (emit, callback)](#apidoc.element.mongoose.connection.prototype._open)
- description and source-code
```javascript
_open = function (emit, callback) {
  this.readyState = STATES.connecting;
  this._closeCalled = false;

  var _this = this;

  var method = this.replica
      ? 'doOpenSet'
      : 'doOpen';

  // open connection
  this[method](function(err) {
    if (err) {
      _this.readyState = STATES.disconnected;
      if (_this._hasOpened) {
        if (callback) {
          callback(err);
        }
      } else {
        _this.error(err, emit && callback);
      }
      return;
    }

    _this.onOpen(callback);
  });
}
```
- example usage
```shell
...

this.name = database;
this.host = host;
this.port = port;

var _this = this;
var promise = new Promise.ES6(function(resolve, reject) {
  _this._open(true, function(error) {
    callback && callback(error);
    if (error) {
      // Error can be on same tick re: christkv/mongodb-core#157
      setImmediate(function() {
        reject(error);
        if (!callback && !promise.$hasHandler) {
          _this.emit('error', error);
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.authMechanismDoesNotRequirePassword"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>authMechanismDoesNotRequirePassword ()](#apidoc.element.mongoose.connection.prototype.authMechanismDoesNotRequirePassword)
- description and source-code
```javascript
authMechanismDoesNotRequirePassword = function () {
  if (this.options && this.options.auth) {
    return authMechanismsWhichDontRequirePassword.indexOf(this.options.auth.authMechanism) >= 0;
  }
  return true;
}
```
- example usage
```shell
...
* username and password are both provided than authentication is needed, but in some cases a
* password is not required.
* @api private
* @return {Boolean} true if the connection should be authenticated after it is opened, otherwise false.
*/
Connection.prototype.shouldAuthenticate = function() {
 return (this.user !== null && this.user !== void 0) &&
     ((this.pass !== null || this.pass !== void 0) || this.authMechanismDoesNotRequirePassword());
};

/**
* @brief Returns a boolean value that specifies if the current authentication mechanism needs a
* password to authenticate according to the auth objects passed into the open/openSet methods.
* @api private
* @return {Boolean} true if the authentication mechanism specified in the options object requires
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.close"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>close (callback)](#apidoc.element.mongoose.connection.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  var _this = this;
  var Promise = PromiseProvider.get();
  return new Promise.ES6(function(resolve, reject) {
    _this._close(function(error) {
      callback && callback(error);
      if (error) {
        reject(error);
        return;
      }
      resolve();
    });
  });
}
```
- example usage
```shell
...
* For practical reasons, a Connection equals a Db.
*
* @param {Mongoose} base a mongoose instance
* @inherits NodeJS EventEmitter http://nodejs.org/api/events.html#events_class_events_eventemitter
* @event 'connecting': Emitted when 'connection.{open,openSet}()' is executed on this connection.
* @event 'connected': Emitted when this connection successfully connects to the db. May be emitted _multiple_ times in 'reconnected
' scenarios.
* @event 'open': Emitted after we 'connected' and 'onOpen' is executed on all of this connections models.
* @event 'disconnecting': Emitted when 'connection.close()' was executed.
* @event 'disconnected': Emitted after getting disconnected from the db.
* @event 'close': Emitted after we 'disconnected' and 'onClose' executed on all of this connections models.
* @event 'reconnected': Emitted after we 'connected' and subsequently 'disconnected', followed by successfully another successfull
 connection.
* @event 'error': Emitted when an error occurs on this connection.
* @event 'fullsetup': Emitted in a replica-set scenario, when primary and at least one seconaries specified in the connection string
 are connected.
* @event 'all': Emitted in a replica-set scenario, when all nodes specified in the connection string are connected.
* @api public
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.collection"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>collection (name, options)](#apidoc.element.mongoose.connection.prototype.collection)
- description and source-code
```javascript
collection = function (name, options) {
  if (!(name in this.collections)) {
    this.collections[name] = new Collection(name, this, options);
  }
  return this.collections[name];
}
```
- example usage
```shell
...
model.prototype.$__setSchema(schema);

var collectionOptions = {
  bufferCommands: schema.options.bufferCommands,
  capped: schema.options.capped
};

model.prototype.collection = connection.collection(
    collectionName
    , collectionOptions
);

// apply methods and statics
applyMethods(model, schema);
applyStatics(model, schema);
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.dropDatabase"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>dropDatabase (callback)](#apidoc.element.mongoose.connection.prototype.dropDatabase)
- description and source-code
```javascript
dropDatabase = function (callback) {
  var Promise = PromiseProvider.get();
  var _this = this;
  var promise = new Promise.ES6(function(resolve, reject) {
    if (_this.readyState !== STATES.connected) {
      _this.on('open', function() {
        _this.db.dropDatabase(function(error) {
          if (error) {
            reject(error);
          } else {
            resolve();
          }
        });
      });
    } else {
      _this.db.dropDatabase(function(error) {
        if (error) {
          reject(error);
        } else {
          resolve();
        }
      });
    }
  });
  if (callback) {
    promise.then(function() { callback(); }, callback);
  }
  return promise;
}
```
- example usage
```shell
...

Connection.prototype.dropDatabase = function(callback) {
var Promise = PromiseProvider.get();
var _this = this;
var promise = new Promise.ES6(function(resolve, reject) {
  if (_this.readyState !== STATES.connected) {
    _this.on('open', function() {
      _this.db.dropDatabase(function(error) {
        if (error) {
          reject(error);
        } else {
          resolve();
        }
      });
    });
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.error"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>error (err, callback)](#apidoc.element.mongoose.connection.prototype.error)
- description and source-code
```javascript
error = function (err, callback) {
  if (callback) {
    return callback(err);
  }
  this.emit('error', err);
}
```
- example usage
```shell
...
if (!rgxProtocol.test(host)) {
  host = 'mongodb://' + host;
}

try {
  parsed = muri(host);
} catch (err) {
  this.error(err, callback);
  return new Promise.ES6(function(resolve, reject) {
    reject(err);
  });
}

database = parsed.db;
host = parsed.hosts[0].host || parsed.hosts[0].ipc;
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.model"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>model (name, schema, collection)](#apidoc.element.mongoose.connection.prototype.model)
- description and source-code
```javascript
model = function (name, schema, collection) {
  // collection name discovery
  if (typeof schema === 'string') {
    collection = schema;
    schema = false;
  }

  if (utils.isObject(schema) && !schema.instanceOfSchema) {
    schema = new Schema(schema);
  }
  if (schema && !schema.instanceOfSchema) {
    throw new Error('The 2nd parameter to 'mongoose.model()' should be a ' +
      'schema or a POJO');
  }

  if (this.models[name] && !collection) {
    // model exists but we are not subclassing with custom collection
    if (schema && schema.instanceOfSchema && schema !== this.models[name].schema) {
      throw new MongooseError.OverwriteModelError(name);
    }
    return this.models[name];
  }

  var opts = {cache: false, connection: this};
  var model;

  if (schema && schema.instanceOfSchema) {
    // compile a model
    model = this.base.model(name, schema, collection, opts);

    // only the first model with this name is cached to allow
    // for one-offs with custom collection names etc.
    if (!this.models[name]) {
      this.models[name] = model;
    }

    model.init();
    return model;
  }

  if (this.models[name] && collection) {
    // subclassing current model with alternate collection
    model = this.models[name];
    schema = model.prototype.schema;
    var sub = model.__subclass(this, schema, collection);
    // do not cache the sub model
    return sub;
  }

  // lookup model in mongoose module
  model = this.base.models[name];

  if (!model) {
    throw new MongooseError.MissingSchemaError(name);
  }

  if (this === model.prototype.db
      && (!collection || collection === model.collection.name)) {
    // model already uses this connection.

    // only the first model with this name is cached to allow
    // for one-offs with custom collection names etc.
    if (!this.models[name]) {
      this.models[name] = model;
    }

    return model;
  }
  this.models[name] = model.__subclass(this, schema, collection);
  return this.models[name];
}
```
- example usage
```shell
...
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model

Once we define a model through 'mongoose.model('ModelName', mySchema)', we can access it through the same function

'''js
var myModel = mongoose.model('ModelName');
'''

Or just do it all at once
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.modelNames"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>modelNames ()](#apidoc.element.mongoose.connection.prototype.modelNames)
- description and source-code
```javascript
modelNames = function () {
  return Object.keys(this.models);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.connection.prototype.onClose"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>onClose ()](#apidoc.element.mongoose.connection.prototype.onClose)
- description and source-code
```javascript
onClose = function () {
  this.readyState = STATES.disconnected;

  // avoid having the collection subscribe to our event emitter
  // to prevent 0.3 warning
  for (var i in this.collections) {
    if (utils.object.hasOwnProperty(this.collections, i)) {
      this.collections[i].onClose();
    }
  }

  this.emit('close');
}
```
- example usage
```shell
...
case 1: // connected
case 4: // unauthorized
  this.readyState = STATES.disconnecting;
  this.doClose(function(err) {
    if (err) {
      _this.error(err, callback);
    } else {
      _this.onClose();
      callback && callback();
    }
  });
  break;

case 2: // connecting
  this.once('open', function() {
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.onOpen"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>onOpen (callback)](#apidoc.element.mongoose.connection.prototype.onOpen)
- description and source-code
```javascript
onOpen = function (callback) {
  var _this = this;

  function open(err, isAuth) {
    if (err) {
      _this.readyState = isAuth ? STATES.unauthorized : STATES.disconnected;
      _this.error(err, callback);
      return;
    }

    _this.readyState = STATES.connected;

    // avoid having the collection subscribe to our event emitter
    // to prevent 0.3 warning
    for (var i in _this.collections) {
      if (utils.object.hasOwnProperty(_this.collections, i)) {
        _this.collections[i].onOpen();
      }
    }

    callback && callback();
    _this.emit('open');
  }

  // re-authenticate if we're not already connected #3871
  if (this._readyState !== STATES.connected && this.shouldAuthenticate()) {
    _this.db.authenticate(_this.user, _this.pass, _this.options.auth, function(err) {
      open(err, true);
    });
  } else {
    open();
  }
}
```
- example usage
```shell
...
 this.collectionName = name;
 this.conn = conn;
 this.queue = [];
 this.buffer = this.opts.bufferCommands;
 this.emitter = new EventEmitter();

 if (STATES.connected === this.conn.readyState) {
   this.onOpen();
 }
}

/**
* The collection name
*
* @api public
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.open"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>open (host, database, port, options, callback)](#apidoc.element.mongoose.connection.prototype.open)
- description and source-code
```javascript
open = function (host, database, port, options, callback) {
  var parsed;
  var Promise = PromiseProvider.get();

  if (typeof database === 'string') {
    switch (arguments.length) {
      case 2:
        port = 27017;
        break;
      case 3:
        switch (typeof port) {
          case 'function':
            callback = port;
            port = 27017;
            break;
          case 'object':
            options = port;
            port = 27017;
            break;
        }
        break;
      case 4:
        if (typeof options === 'function') {
          callback = options;
          options = {};
        }
    }
  } else {
    switch (typeof database) {
      case 'function':
        callback = database;
        database = undefined;
        break;
      case 'object':
        options = database;
        database = undefined;
        callback = port;
        break;
    }

    if (!rgxProtocol.test(host)) {
      host = 'mongodb://' + host;
    }

    try {
      parsed = muri(host);
    } catch (err) {
      this.error(err, callback);
      return new Promise.ES6(function(resolve, reject) {
        reject(err);
      });
    }

    database = parsed.db;
    host = parsed.hosts[0].host || parsed.hosts[0].ipc;
    port = parsed.hosts[0].port || 27017;
  }

  this.options = this.parseOptions(options, parsed && parsed.options);

  // make sure we can open
  if (STATES.disconnected !== this.readyState) {
    var err = new Error('Trying to open unclosed connection.');
    err.state = this.readyState;
    this.error(err, callback);
    return new Promise.ES6(function(resolve, reject) {
      reject(err);
    });
  }

  if (!host) {
    this.error(new Error('Missing hostname.'), callback);
    return new Promise.ES6(function(resolve, reject) {
      reject(err);
    });
  }

  if (!database) {
    this.error(new Error('Missing database name.'), callback);
    return new Promise.ES6(function(resolve, reject) {
      reject(err);
    });
  }

  // authentication
  if (this.optionsProvideAuthenticationData(options)) {
    this.user = options.user;
    this.pass = options.pass;
  } else if (parsed && parsed.auth) {
    this.user = parsed.auth.user;
    this.pass = parsed.auth.pass;

    // Check hostname for user/pass
  } else if (/@/.test(host) && /:/.test(host.split('@')[0])) {
    host = host.split('@');
    var auth = host.shift().split(':');
    host = host.pop();
    this.user = auth[0];
    this.pass = auth[1];
  } else {
    this.user = this.pass = undefined;
  }

  // global configuration options
  if (options && options.config) {
    this.config.autoIndex = options.config.autoIndex !== false;
  }

  this.name = database;
  this.host = host;
  this.port = port;

  var _this = this;
  var promise = new Promise.ES6(function(resolve, reject) {
    _this._open(true, function(error) {
      callback && callback(error);
      if (error) {
        // Error can be on same tick re: christkv/mongodb-core#157
        setImmediate(function() {
          reject(error);
          if (!callback && !promise.$hasHandler) {
            _this.emit('error', error);
          }
        });
        return;
      }
      resolve();
    });
  });
  return promise;
}
```
- example usage
```shell
...
*
* _Options passed take precedence over options included in connection strings._
*
* ####Notes:
*
* _If connecting to multiple mongos servers, set the 'mongos' option to true._
*
*     conn.open('mongodb://mongosA:27501,mongosB:27501', { mongos: true }, cb);
*
* Mongoose forces the db option 'forceServerObjectId' false and cannot be overridden.
* Mongoose defaults the server 'auto_reconnect' options to true which can be overridden.
* See the node-mongodb-native driver instance for options that it understands.
*
* _Options passed take precedence over options included in connection strings._
*
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.openSet"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>openSet (uris, database, options, callback)](#apidoc.element.mongoose.connection.prototype.openSet)
- description and source-code
```javascript
openSet = function (uris, database, options, callback) {
  if (!rgxProtocol.test(uris)) {
    uris = 'mongodb://' + uris;
  }

  var Promise = PromiseProvider.get();

  switch (arguments.length) {
    case 3:
      switch (typeof database) {
        case 'string':
          this.name = database;
          break;
        case 'object':
          callback = options;
          options = database;
          database = null;
          break;
      }

      if (typeof options === 'function') {
        callback = options;
        options = {};
      }
      break;
    case 2:
      switch (typeof database) {
        case 'string':
          this.name = database;
          break;
        case 'function':
          callback = database;
          database = null;
          break;
        case 'object':
          options = database;
          database = null;
          break;
      }
  }

  if (typeof database === 'string') {
    this.name = database;
  }

  var parsed;
  try {
    parsed = muri(uris);
  } catch (err) {
    this.error(err, callback);
    return new Promise.ES6(function(resolve, reject) {
      reject(err);
    });
  }

  if (!this.name) {
    this.name = parsed.db;
  }

  this.hosts = parsed.hosts;
  this.options = this.parseOptions(options, parsed && parsed.options);
  this.replica = true;

  if (!this.name) {
    var err = new Error('No database name provided for replica set');
    this.error(err, callback);
    return new Promise.ES6(function(resolve, reject) {
      reject(err);
    });
  }

  // authentication
  if (this.optionsProvideAuthenticationData(options)) {
    this.user = options.user;
    this.pass = options.pass;
  } else if (parsed && parsed.auth) {
    this.user = parsed.auth.user;
    this.pass = parsed.auth.pass;
  } else {
    this.user = this.pass = undefined;
  }

  // global configuration options
  if (options && options.config) {
    this.config.autoIndex = options.config.autoIndex !== false;
  }

  var _this = this;
  var emitted = false;
  var promise = new Promise.ES6(function(resolve, reject) {
    _this._open(true, function(error) {
      callback && callback(error);
      if (error) {
        reject(error);
        if (!callback && !promise.$hasHandler && !emitted) {
          emitted = true;
          _this.emit('error', error);
        }
        return;
      }
      resolve();
    });
  });
  return promise;
}
```
- example usage
```shell
...

/**
* Opens the connection to a replica set.
*
* ####Example:
*
*     var db = mongoose.createConnection();
*     db.openSet("mongodb://user:pwd@localhost:27020,localhost:27021,localhost:27012/mydb");
*
* The database name and/or auth need only be included in one URI.
* The 'options' is a hash which is passed to the internal driver connection object.
*
* Valid 'options'
*
*     db      - passed to the connection db instance
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.optionsProvideAuthenticationData"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>optionsProvideAuthenticationData (options)](#apidoc.element.mongoose.connection.prototype.optionsProvideAuthenticationData)
- description and source-code
```javascript
optionsProvideAuthenticationData = function (options) {
  return (options) &&
      (options.user) &&
      ((options.pass) || this.authMechanismDoesNotRequirePassword());
}
```
- example usage
```shell
...
this.error(new Error('Missing database name.'), callback);
return new Promise.ES6(function(resolve, reject) {
  reject(err);
});
  }

  // authentication
  if (this.optionsProvideAuthenticationData(options)) {
this.user = options.user;
this.pass = options.pass;
  } else if (parsed && parsed.auth) {
this.user = parsed.auth.user;
this.pass = parsed.auth.pass;

// Check hostname for user/pass
...
```

#### <a name="apidoc.element.mongoose.connection.prototype.shouldAuthenticate"></a>[function <span class="apidocSignatureSpan">mongoose.connection.prototype.</span>shouldAuthenticate ()](#apidoc.element.mongoose.connection.prototype.shouldAuthenticate)
- description and source-code
```javascript
shouldAuthenticate = function () {
  return (this.user !== null && this.user !== void 0) &&
      ((this.pass !== null || this.pass !== void 0) || this.authMechanismDoesNotRequirePassword());
}
```
- example usage
```shell
...
    }

    callback && callback();
    _this.emit('open');
  }

  // re-authenticate if we're not already connected #3871
  if (this._readyState !== STATES.connected && this.shouldAuthenticate()) {
    _this.db.authenticate(_this.user, _this.pass, _this.options.auth, function(err) {
      open(err, true);
    });
  } else {
    open();
  }
};
...
```



# <a name="apidoc.module.mongoose.document"></a>[module mongoose.document](#apidoc.module.mongoose.document)

#### <a name="apidoc.element.mongoose.document.document"></a>[function <span class="apidocSignatureSpan">mongoose.</span>document (obj, fields, skipId)](#apidoc.element.mongoose.document.document)
- description and source-code
```javascript
function Document(obj, fields, skipId) {
  this.$__ = new InternalCache;
  this.$__.emitter = new EventEmitter();
  this.isNew = true;
  this.errors = undefined;

  var schema = this.schema;

  if (typeof fields === 'boolean') {
    this.$__.strictMode = fields;
    fields = undefined;
  } else {
    this.$__.strictMode = schema.options && schema.options.strict;
    this.$__.selected = fields;
  }

  var required = schema.requiredPaths(true);
  for (var i = 0; i < required.length; ++i) {
    this.$__.activePaths.require(required[i]);
  }

  this.$__.emitter.setMaxListeners(0);
  this._doc = this.$__buildDoc(obj, fields, skipId);

  if (obj) {
    if (obj instanceof Document) {
      this.isNew = obj.isNew;
    }
    // Skip set hooks
    if (this.$__original_set) {
      this.$__original_set(obj, undefined, true);
    } else {
      this.set(obj, undefined, true);
    }
  }

  if (!schema.options.strict && obj) {
    var _this = this,
        keys = Object.keys(this._doc);

    keys.forEach(function(key) {
      if (!(key in schema.tree)) {
        defineKey(key, null, _this);
      }
    });
  }

  applyQueue(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.ValidationError"></a>[function <span class="apidocSignatureSpan">mongoose.document.</span>ValidationError (instance)](#apidoc.element.mongoose.document.ValidationError)
- description and source-code
```javascript
function ValidationError(instance) {
  this.errors = {};
  if (instance && instance.constructor.name === 'model') {
    MongooseError.call(this, instance.constructor.modelName + ' validation failed');
  } else {
    MongooseError.call(this, 'Validation failed');
  }
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.name = 'ValidationError';
  if (instance) {
    instance.errors = this.errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document._lazySetupHooks"></a>[function <span class="apidocSignatureSpan">mongoose.document.</span>_lazySetupHooks (proto, methodName, errorCb)](#apidoc.element.mongoose.document._lazySetupHooks)
- description and source-code
```javascript
_lazySetupHooks = function (proto, methodName, errorCb) {
  if ('undefined' === typeof proto[methodName].numAsyncPres) {
    this.$hook(methodName, proto[methodName], errorCb);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.removePost"></a>[function <span class="apidocSignatureSpan">mongoose.document.</span>removePost (name, fnToRemove)](#apidoc.element.mongoose.document.removePost)
- description and source-code
```javascript
removePost = function (name, fnToRemove) {
  var proto = this.prototype || this
    , posts = proto._posts || (proto._posts || {});
  if (!posts[name]) return this;
  if (arguments.length === 1) {
    // Remove all post callbacks for hook 'name'
    posts[name].length = 0;
  } else {
    posts[name] = posts[name].filter( function (currFn) {
      return currFn !== fnToRemove;
    });
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.removePre"></a>[function <span class="apidocSignatureSpan">mongoose.document.</span>removePre (name, fnToRemove)](#apidoc.element.mongoose.document.removePre)
- description and source-code
```javascript
removePre = function (name, fnToRemove) {
  var proto = this.prototype || this
    , pres = proto._pres || (proto._pres || {});
  if (!pres[name]) return this;
  if (arguments.length === 1) {
    // Remove all pre callbacks for hook 'name'
    pres[name].length = 0;
  } else {
    pres[name] = pres[name].filter( function (currFn) {
      return currFn !== fnToRemove;
    });
  }
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.document.prototype"></a>[module mongoose.document.prototype](#apidoc.module.mongoose.document.prototype)

#### <a name="apidoc.element.mongoose.document.prototype._lazySetupHooks"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>_lazySetupHooks (proto, methodName, errorCb)](#apidoc.element.mongoose.document.prototype._lazySetupHooks)
- description and source-code
```javascript
_lazySetupHooks = function (proto, methodName, errorCb) {
  if ('undefined' === typeof proto[methodName].numAsyncPres) {
    this.$hook(methodName, proto[methodName], errorCb);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.addListener"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>addListener ()](#apidoc.element.mongoose.document.prototype.addListener)
- description and source-code
```javascript
addListener = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.depopulate"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>depopulate (path)](#apidoc.element.mongoose.document.prototype.depopulate)
- description and source-code
```javascript
depopulate = function (path) {
  var populatedIds = this.populated(path);
  if (!populatedIds) {
    return;
  }
  delete this.$__.populated[path];
  this.set(path, populatedIds);
  return this;
}
```
- example usage
```shell
...
/**
* Takes a populated field and returns it to its unpopulated state.
*
* ####Example:
*
*     Model.findOne().populate('author').exec(function (err, doc) {
*       console.log(doc.author.name); // Dr.Seuss
*       console.log(doc.depopulate('author'));
*       console.log(doc.author); // '5144cf8050f071d979c118a7'
*     })
*
* If the path was not populated, this is a no-op.
*
* @param {String} path
* @return {Document} this
...
```

#### <a name="apidoc.element.mongoose.document.prototype.emit"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>emit ()](#apidoc.element.mongoose.document.prototype.emit)
- description and source-code
```javascript
emit = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
...
You can intercept method arguments via middleware.

For example, this would allow you to broadcast changes about your Documents every time someone 'set's a path in your Document to
 a new value:

'''js
schema.pre('set', function (next, path, val, typel) {
  // 'this' is the current Document
  this.emit('set', path, val);

  // Pass control to the next pre
  next();
});
'''

Moreover, you can mutate the incoming 'method' arguments so that subsequent middleware see different values for those arguments.
To do so, just pass the new values to 'next':
...
```

#### <a name="apidoc.element.mongoose.document.prototype.equals"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>equals (doc)](#apidoc.element.mongoose.document.prototype.equals)
- description and source-code
```javascript
equals = function (doc) {
  if (!doc) {
    return false;
  }

  var tid = this.get('_id');
  var docid = doc.get ? doc.get('_id') : doc;
  if (!tid && !docid) {
    return deepEqual(this, doc);
  }
  return tid && tid.equals
      ? tid.equals(docid)
      : tid === docid;
}
```
- example usage
```shell
...

 var tid = this.get('_id');
 var docid = doc.get ? doc.get('_id') : doc;
 if (!tid && !docid) {
   return deepEqual(this, doc);
 }
 return tid && tid.equals
     ? tid.equals(docid)
     : tid === docid;
};

/**
* Populates document references, executing the 'callback' when complete.
* If you want to use promises instead, use this function with
* ['execPopulate()'](#document_Document-execPopulate)
...
```

#### <a name="apidoc.element.mongoose.document.prototype.execPopulate"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>execPopulate ()](#apidoc.element.mongoose.document.prototype.execPopulate)
- description and source-code
```javascript
execPopulate = function () {
  var Promise = PromiseProvider.get();
  var _this = this;
  return new Promise.ES6(function(resolve, reject) {
    _this.populate(function(error, res) {
      if (error) {
        reject(error);
      } else {
        resolve(res);
      }
    });
  });
}
```
- example usage
```shell
...
*
*     // summary
*     doc.populate(path)                   // not executed
*     doc.populate(options);               // not executed
*     doc.populate(path, callback)         // executed
*     doc.populate(options, callback);     // executed
*     doc.populate(callback);              // executed
*     doc.populate(options).execPopulate() // executed, returns promise
*
*
* ####NOTE:
*
* Population does not occur unless a 'callback' is passed *or* you explicitly
* call 'execPopulate()'.
* Passing the same path a second time will overwrite the previous path options.
...
```

#### <a name="apidoc.element.mongoose.document.prototype.get"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>get (path, type)](#apidoc.element.mongoose.document.prototype.get)
- description and source-code
```javascript
get = function (path, type) {
  var adhoc;
  if (type) {
    adhoc = Schema.interpretAsType(path, type, this.schema.options);
  }

  var schema = this.$__path(path) || this.schema.virtualpath(path),
      pieces = path.split('.'),
      obj = this._doc;

  for (var i = 0, l = pieces.length; i < l; i++) {
    obj = obj === null || obj === void 0
        ? undefined
        : obj[pieces[i]];
  }

  if (adhoc) {
    obj = adhoc.cast(obj);
  }

  // Check if this path is populated - don't apply getters if it is,
  // because otherwise its a nested object. See gh-3357
  if (schema && !this.populated(path)) {
    obj = schema.applyGetters(obj, this);
  }

  return obj;
}
```
- example usage
```shell
...
// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model
...
```

#### <a name="apidoc.element.mongoose.document.prototype.getValue"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>getValue (path)](#apidoc.element.mongoose.document.prototype.getValue)
- description and source-code
```javascript
getValue = function (path) {
  return utils.getValue(path, this._doc);
}
```
- example usage
```shell
...
// If doc._id is not null or undefined
if (doc._id !== null && doc._id !== undefined &&
  opts && opts.populated && opts.populated.length) {
  var id = String(doc._id);
  for (var i = 0; i < opts.populated.length; ++i) {
    var item = opts.populated[i];
    if (item.isVirtual) {
      this.populated(item.path, utils.getValue(item.path, doc), item);
    } else {
      this.populated(item.path, item._docs[id], item);
    }
  }
}

init(this, doc, this._doc);
...
```

#### <a name="apidoc.element.mongoose.document.prototype.init"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>init (doc, opts, fn)](#apidoc.element.mongoose.document.prototype.init)
- description and source-code
```javascript
init = function (doc, opts, fn) {
  // do not prefix this method with $__ since its
  // used by public hooks

  if (typeof opts === 'function') {
    fn = opts;
    opts = null;
  }

  this.isNew = false;

  // handle docs with populated paths
  // If doc._id is not null or undefined
  if (doc._id !== null && doc._id !== undefined &&
    opts && opts.populated && opts.populated.length) {
    var id = String(doc._id);
    for (var i = 0; i < opts.populated.length; ++i) {
      var item = opts.populated[i];
      if (item.isVirtual) {
        this.populated(item.path, utils.getValue(item.path, doc), item);
      } else {
        this.populated(item.path, item._docs[id], item);
      }
    }
  }

  init(this, doc, this._doc);
  this.$__storeShard();

  this.emit('init', this);
  this.constructor.emit('init', this);

  if (fn) {
    fn(null);
  }
  return this;
}
```
- example usage
```shell
...
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);

if (!skipInit && obj) {
  this.init(obj);
}

this.$__registerHooksFromSchema();

// apply methods
for (var m in schema.methods) {
  this[m] = schema.methods[m];
...
```

#### <a name="apidoc.element.mongoose.document.prototype.inspect"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>inspect (options)](#apidoc.element.mongoose.document.prototype.inspect)
- description and source-code
```javascript
inspect = function (options) {
  var isPOJO = options &&
    utils.getFunctionName(options.constructor) === 'Object';
  var opts;
  if (isPOJO) {
    opts = options;
    opts.minimize = false;
    opts.retainKeyOrder = true;
  }
  return this.toObject(opts);
}
```
- example usage
```shell
...
* Helper for console.log
*
* @api public
* @method toString
*/

Document.prototype.toString = function() {
 return inspect(this.inspect());
};

/**
* Returns true if the Document stores the same data as doc.
*
* Documents are considered equal when they have matching '_id's, unless neither
* document has an '_id', in which case this function falls back to using
...
```

#### <a name="apidoc.element.mongoose.document.prototype.invalidate"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>invalidate (path, err, val, kind)](#apidoc.element.mongoose.document.prototype.invalidate)
- description and source-code
```javascript
invalidate = function (path, err, val, kind) {
  if (!this.$__.validationError) {
    this.$__.validationError = new ValidationError(this);
  }

  if (this.$__.validationError.errors[path]) {
    return;
  }

  if (!err || typeof err === 'string') {
    err = new ValidatorError({
      path: path,
      message: err,
      type: kind || 'user defined',
      value: val
    });
  }

  if (this.$__.validationError === err) {
    return this.$__.validationError;
  }

  this.$__.validationError.errors[path] = err;
  return this.$__.validationError;
}
```
- example usage
```shell
...
if (obj[i] === null) {
  doc[i] = null;
} else if (obj[i] !== undefined) {
  if (schema) {
    try {
      doc[i] = schema.cast(obj[i], self, true);
    } catch (e) {
      self.invalidate(e.path, new ValidatorError({
        path: e.path,
        message: e.message,
        type: 'cast',
        value: e.value
      }));
    }
  } else {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.isDirectModified"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isDirectModified (path)](#apidoc.element.mongoose.document.prototype.isDirectModified)
- description and source-code
```javascript
isDirectModified = function (path) {
  return (path in this.$__.activePaths.states.modify);
}
```
- example usage
```shell
...
// Else mongodb throws: "LEFT_SUBFIELD only supports Object"

if (parts.length <= 1) {
  pathToMark = path;
} else {
  for (i = 0; i < parts.length; ++i) {
    subpath = parts.slice(0, i + 1).join('.');
    if (this.isDirectModified(subpath) // earlier prefixes that are already
          // marked as dirty have precedence
        || this.get(subpath) === null) {
      pathToMark = subpath;
      break;
    }
  }
...
```

#### <a name="apidoc.element.mongoose.document.prototype.isInit"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isInit (path)](#apidoc.element.mongoose.document.prototype.isInit)
- description and source-code
```javascript
isInit = function (path) {
  return (path in this.$__.activePaths.states.init);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.isModified"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isModified (paths)](#apidoc.element.mongoose.document.prototype.isModified)
- description and source-code
```javascript
isModified = function (paths) {
  if (paths) {
    if (!Array.isArray(paths)) {
      paths = paths.split(' ');
    }
    var modified = this.modifiedPaths();
    var directModifiedPaths = Object.keys(this.$__.activePaths.states.modify);
    var isModifiedChild = paths.some(function(path) {
      return !!~modified.indexOf(path);
    });
    return isModifiedChild || paths.some(function(path) {
      return directModifiedPaths.some(function(mod) {
        return mod === path || path.indexOf(mod + '.') === 0;
      });
    });
  }
  return this.$__.activePaths.some('modify');
}
```
- example usage
```shell
...
            }));
          }
        } else {
          doc[i] = obj[i];
        }
      }
      // mark as hydrated
      if (!self.isModified(path)) {
        self.$__.activePaths.init(path);
      }
    }
  }
}

/**
...
```

#### <a name="apidoc.element.mongoose.document.prototype.isSelected"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>isSelected (path)](#apidoc.element.mongoose.document.prototype.isSelected)
- description and source-code
```javascript
function isSelected(path) {
  if (this.$__.selected) {
    if (path === '_id') {
      return this.$__.selected._id !== 0;
    }

    var paths = Object.keys(this.$__.selected);
    var i = paths.length;
    var inclusive = null;
    var cur;

    if (i === 1 && paths[0] === '_id') {
      // only _id was selected.
      return this.$__.selected._id === 0;
    }

    while (i--) {
      cur = paths[i];
      if (cur === '_id') {
        continue;
      }
      if (this.$__.selected[cur] && this.$__.selected[cur].$meta) {
        continue;
      }
      inclusive = !!this.$__.selected[cur];
      break;
    }

    if (inclusive === null) {
      return true;
    }

    if (path in this.$__.selected) {
      return inclusive;
    }

    i = paths.length;
    var pathDot = path + '.';

    while (i--) {
      cur = paths[i];
      if (cur === '_id') {
        continue;
      }

      if (cur.indexOf(pathDot) === 0) {
        return inclusive || cur !== pathDot;
      }

      if (pathDot.indexOf(cur + '.') === 0) {
        return inclusive;
      }
    }

    return !inclusive;
  }

  return true;
}
```
- example usage
```shell
...
i = keys[index];
path = prefix + i;
schema = self.schema.path(path);

// Should still work if not a model-level discriminator, but should not be
// necessary. This is *only* to catch the case where we queried using the
// base model and the discriminated model has a projection
if (self.schema.$isRootDiscriminator && !self.isSelected(path)) {
  return;
}

if (!schema && utils.isObject(obj[i]) &&
    (!obj[i].constructor || utils.getFunctionName(obj[i].constructor) === 'Object')) {
  // assume nested object
  if (!doc[i]) {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.listeners"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>listeners ()](#apidoc.element.mongoose.document.prototype.listeners)
- description and source-code
```javascript
listeners = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
...
      doc[pair[0]].apply(doc, pair[1]);
    }
  }
}

Document.prototype.$__handleReject = function handleReject(err) {
  // emit on the Model if listening
  if (this.listeners('error').length) {
    this.emit('error', err);
  } else if (this.constructor.listeners && this.constructor.listeners('error').length) {
    this.constructor.emit('error', err);
  } else if (this.listeners && this.listeners('error').length) {
    this.emit('error', err);
  }
};
...
```

#### <a name="apidoc.element.mongoose.document.prototype.markModified"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>markModified (path)](#apidoc.element.mongoose.document.prototype.markModified)
- description and source-code
```javascript
markModified = function (path) {
  this.$__.activePaths.modify(path);
}
```
- example usage
```shell
...
  if (!merge) {
    this.setValue(path, null);
    cleanModifiedSubpaths(this, path);
  }

  if (Object.keys(val).length === 0) {
    this.setValue(path, {});
    this.markModified(path);
    cleanModifiedSubpaths(this, path);
  } else {
    this.set(val, path, constructing);
  }
  return this;
}
this.invalidate(path, new MongooseError.CastError('Object', val, path));
...
```

#### <a name="apidoc.element.mongoose.document.prototype.modifiedPaths"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>modifiedPaths ()](#apidoc.element.mongoose.document.prototype.modifiedPaths)
- description and source-code
```javascript
modifiedPaths = function () {
  var directModifiedPaths = Object.keys(this.$__.activePaths.states.modify);
  return directModifiedPaths.reduce(function(list, path) {
    var parts = path.split('.');
    return list.concat(parts.reduce(function(chains, part, i) {
      return chains.concat(parts.slice(0, i).concat(part).join('.'));
    }, []).filter(function(chain) {
      return (list.indexOf(chain) === -1);
    }));
  }, []);
}
```
- example usage
```shell
...
 */

Document.prototype.isModified = function(paths) {
if (paths) {
  if (!Array.isArray(paths)) {
    paths = paths.split(' ');
  }
  var modified = this.modifiedPaths();
  var directModifiedPaths = Object.keys(this.$__.activePaths.states.modify);
  var isModifiedChild = paths.some(function(path) {
    return !!~modified.indexOf(path);
  });
  return isModifiedChild || paths.some(function(path) {
    return directModifiedPaths.some(function(mod) {
      return mod === path || path.indexOf(mod + '.') === 0;
...
```

#### <a name="apidoc.element.mongoose.document.prototype.on"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>on ()](#apidoc.element.mongoose.document.prototype.on)
- description and source-code
```javascript
on = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
...
 * - 2 = connecting
 * - 3 = disconnecting
 *
 * Each state change emits its associated event name.
 *
 * ####Example
 *
 *     conn.on('connected', callback);
 *     conn.on('disconnected', callback);
 *
 * @property readyState
 * @api public
 */

Object.defineProperty(Connection.prototype, 'readyState', {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.once"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>once ()](#apidoc.element.mongoose.document.prototype.once)
- description and source-code
```javascript
once = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
...
        aggregate(_this._pipeline, options || {});
      decorateCursor(cursor);
      resolve(cursor);
      callback && callback(null, cursor);
    });
    return;
  }
  _this._model.collection.emitter.once('queue', function() {
    var cursor = _this._model.collection.
      aggregate(_this._pipeline, options || {});
    decorateCursor(cursor);
    resolve(cursor);
    callback && callback(null, cursor);
  });
});
...
```

#### <a name="apidoc.element.mongoose.document.prototype.populate"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>populate ()](#apidoc.element.mongoose.document.prototype.populate)
- description and source-code
```javascript
function populate() {
  if (arguments.length === 0) {
    return this;
  }

  var pop = this.$__.populate || (this.$__.populate = {});
  var args = utils.args(arguments);
  var fn;

  if (typeof args[args.length - 1] === 'function') {
    fn = args.pop();
  }

  // allow 'doc.populate(callback)'
  if (args.length) {
    // use hash to remove duplicate paths
    var res = utils.populate.apply(null, args);
    for (var i = 0; i < res.length; ++i) {
      pop[res[i].path] = res[i];
    }
  }

  if (fn) {
    var paths = utils.object.vals(pop);
    this.$__.populate = undefined;
    paths.__noPromise = true;
    this.constructor.populate(this, paths, fn);
  }

  return this;
}
```
- example usage
```shell
...
* Populates document references, executing the 'callback' when complete.
* If you want to use promises instead, use this function with
* ['execPopulate()'](#document_Document-execPopulate)
*
* ####Example:
*
*     doc
*     .populate('company')
*     .populate({
*       path: 'notes',
*       match: /airline/,
*       select: 'text',
*       model: 'modelName'
*       options: opts
*     }, function (err, user) {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.populated"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>populated (path, val, options)](#apidoc.element.mongoose.document.prototype.populated)
- description and source-code
```javascript
populated = function (path, val, options) {
  // val and options are internal

  if (val === null || val === void 0) {
    if (!this.$__.populated) {
      return undefined;
    }
    var v = this.$__.populated[path];
    if (v) {
      return v.value;
    }
    return undefined;
  }

  // internal

  if (val === true) {
    if (!this.$__.populated) {
      return undefined;
    }
    return this.$__.populated[path];
  }

  this.$__.populated || (this.$__.populated = {});
  this.$__.populated[path] = {value: val, options: options};
  return val;
}
```
- example usage
```shell
...
// If doc._id is not null or undefined
if (doc._id !== null && doc._id !== undefined &&
  opts && opts.populated && opts.populated.length) {
  var id = String(doc._id);
  for (var i = 0; i < opts.populated.length; ++i) {
    var item = opts.populated[i];
    if (item.isVirtual) {
      this.populated(item.path, utils.getValue(item.path, doc), item);
    } else {
      this.populated(item.path, item._docs[id], item);
    }
  }
}

init(this, doc, this._doc);
...
```

#### <a name="apidoc.element.mongoose.document.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removeAllListeners ()](#apidoc.element.mongoose.document.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removeListener ()](#apidoc.element.mongoose.document.prototype.removeListener)
- description and source-code
```javascript
removeListener = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.removePost"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removePost (name, fnToRemove)](#apidoc.element.mongoose.document.prototype.removePost)
- description and source-code
```javascript
removePost = function (name, fnToRemove) {
  var proto = this.prototype || this
    , posts = proto._posts || (proto._posts || {});
  if (!posts[name]) return this;
  if (arguments.length === 1) {
    // Remove all post callbacks for hook 'name'
    posts[name].length = 0;
  } else {
    posts[name] = posts[name].filter( function (currFn) {
      return currFn !== fnToRemove;
    });
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.removePre"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>removePre (name, fnToRemove)](#apidoc.element.mongoose.document.prototype.removePre)
- description and source-code
```javascript
removePre = function (name, fnToRemove) {
  var proto = this.prototype || this
    , pres = proto._pres || (proto._pres || {});
  if (!pres[name]) return this;
  if (arguments.length === 1) {
    // Remove all pre callbacks for hook 'name'
    pres[name].length = 0;
  } else {
    pres[name] = pres[name].filter( function (currFn) {
      return currFn !== fnToRemove;
    });
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.set"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>set (path, val, type, options)](#apidoc.element.mongoose.document.prototype.set)
- description and source-code
```javascript
set = function (path, val, type, options) {
  if (type && utils.getFunctionName(type.constructor) === 'Object') {
    options = type;
    type = undefined;
  }

  var merge = options && options.merge,
      adhoc = type && type !== true,
      constructing = type === true,
      adhocs;

  var strict = options && 'strict' in options
      ? options.strict
      : this.$__.strictMode;

  if (adhoc) {
    adhocs = this.$__.adhocPaths || (this.$__.adhocPaths = {});
    adhocs[path] = Schema.interpretAsType(path, type, this.schema.options);
  }

  if (typeof path !== 'string') {
    // new Document({ key: val })

    if (path === null || path === void 0) {
      var _ = path;
      path = val;
      val = _;
    } else {
      var prefix = val
          ? val + '.'
          : '';

      if (path instanceof Document) {
        if (path.$__isNested) {
          path = path.toObject();
        } else {
          path = path._doc;
        }
      }

      var keys = Object.keys(path);
      var len = keys.length;
      var i = 0;
      var pathtype;
      var key;

      if (len === 0 && !this.schema.options.minimize) {
        if (val) {
          this.set(val, {});
        }
        return this;
      }

      if (this.schema.options.retainKeyOrder) {
        while (i < len) {
          _handleIndex.call(this, i++);
        }
      } else {
        while (len--) {
          _handleIndex.call(this, len);
        }
      }

      return this;
    }
  }

  function _handleIndex(i) {
    key = keys[i];
    var pathName = prefix + key;
    pathtype = this.schema.pathType(pathName);

    if (path[key] !== null
        && path[key] !== void 0
          // need to know if plain object - no Buffer, ObjectId, ref, etc
        && utils.isObject(path[key])
        && (!path[key].constructor || utils.getFunctionName(path[key].constructor) === 'Object')
        && pathtype !== 'virtual'
        && pathtype !== 'real'
        && !(this.$__path(pathName) instanceof MixedSchema)
        && !(this.schema.paths[pathName] &&
        this.schema.paths[pathName].options &&
        this.schema.paths[pathName].options.ref)) {
      this.set(path[key], prefix + key, constructing);
    } else if (strict) {
      // Don't overwrite defaults with undefined keys (gh-3981)
      if (constructing && path[key] === void 0 &&
          this.get(key) !== void 0) {
        return;
      }

      if (pathtype === 'real' || pathtype === 'virtual') {
        // Check for setting single embedded schema to document (gh-3535)
        var p = path[key];
        if (this.schema.paths[pathName] &&
            this.schema.paths[pathName].$isSingleNested &&
            path[key] instanceof Document) {
          p = p.toObject({ virtuals: false, transform: false });
        }
        this.set(prefix + key, p, constructing);
      } else if (pathtype === 'nested' && path[key] instanceof Document) {
        this.set(prefix + key,
            path[key].toObject({transform: false}), constructing);
      } else if (strict === 'throw') {
        if (pathtype === 'nested') {
          throw new ObjectExpectedError(key, path[key]);
        } else {
          throw new StrictModeError(key);
        }
      }
    } else if (path[key] !== void 0) {
      this.set(prefix + key, path[key], constructing);
    }
  }

  var pathType = this.schema.pathType(path);
  if (pathType === 'nested' && val) {
    if (utils.isObject(val) &&
        (!val.constructor || utils.getFunctionName(val.constructor) === 'Object')) {
      if (!merge) {
        this.setValue(path, null);
        cleanModifiedSubpaths(this, path);
      }

      if (Object.keys(val).length === 0) {
        this.setValue(path, {});
        this.markModified(path);
        cleanModifiedSubpaths(this, path);
      } else {
        this.set(val, path, constructing);
      }
      return this;
    }
    this.invalidate(path, new MongooseError.CastError('Object', val, path));
    return this;
  }

  var schema;
  var parts = path.split('.');

  if (pathType === 'adhocOrUndefined' && strict) {
    // check for roots that are Mixed types ...
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```

#### <a name="apidoc.element.mongoose.document.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>setMaxListeners ()](#apidoc.element.mongoose.document.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function () {
  return this.$__.emitter[emitterFn].apply(this.$__.emitter, arguments);
}
```
- example usage
```shell
...
}

var required = this.schema.requiredPaths();
for (var i = 0; i < required.length; ++i) {
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);

if (!skipInit && obj) {
  this.init(obj);
}

this.$__registerHooksFromSchema();
...
```

#### <a name="apidoc.element.mongoose.document.prototype.setValue"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>setValue (path, val)](#apidoc.element.mongoose.document.prototype.setValue)
- description and source-code
```javascript
setValue = function (path, val) {
  utils.setValue(path, val, this._doc);
  return this;
}
```
- example usage
```shell
...
  }

  var pathType = this.schema.pathType(path);
  if (pathType === 'nested' && val) {
    if (utils.isObject(val) &&
  (!val.constructor || utils.getFunctionName(val.constructor) === 'Object')) {
if (!merge) {
  this.setValue(path, null);
  cleanModifiedSubpaths(this, path);
}

if (Object.keys(val).length === 0) {
  this.setValue(path, {});
  this.markModified(path);
  cleanModifiedSubpaths(this, path);
...
```

#### <a name="apidoc.element.mongoose.document.prototype.toBSON"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toBSON ()](#apidoc.element.mongoose.document.prototype.toBSON)
- description and source-code
```javascript
toBSON = function () {
  return this.toObject({
    transform: false,
    virtuals: false,
    _skipDepopulateTopLevel: true,
    depopulate: true,
    flattenDecimals: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.document.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toJSON (options)](#apidoc.element.mongoose.document.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (options) {
  return this.$toObject(options, true);
}
```
- example usage
```shell
...

if (Array.isArray(obj)) {
  return cloneArray(obj, options);
}

if (isMongooseObject(obj)) {
  if (options && options.json && typeof obj.toJSON === 'function') {
    return obj.toJSON(options);
  }
  return obj.toObject(options);
}

if (obj.constructor) {
  switch (exports.getFunctionName(obj.constructor)) {
    case 'Object':
...
```

#### <a name="apidoc.element.mongoose.document.prototype.toObject"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toObject (options)](#apidoc.element.mongoose.document.prototype.toObject)
- description and source-code
```javascript
toObject = function (options) {
  return this.$toObject(options);
}
```
- example usage
```shell
...
  if (value.$maxDistance != null) {
    value.$maxDistance = numbertype.castForQuery(value.$maxDistance);
  }
  if (value.$minDistance != null) {
    value.$minDistance = numbertype.castForQuery(value.$minDistance);
  }
  if (utils.isMongooseObject(value.$geometry)) {
    value.$geometry = value.$geometry.toObject({
      transform: false,
      virtuals: false
    });
  }
  value = value.$geometry.coordinates;
} else if (geo === '$geoWithin') {
  if (value.$geometry) {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>toString ()](#apidoc.element.mongoose.document.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return inspect(this.inspect());
}
```
- example usage
```shell
...
'''

Moreover, you can mutate the incoming 'method' arguments so that subsequent middleware see different values for those arguments.
To do so, just pass the new values to 'next':

'''js
.pre(method, function firstPre (next, methodArg1, methodArg2) {
// Mutate methodArg1
next("altered-" + methodArg1.toString(), methodArg2);
});

// pre declaration is chainable
.pre(method, function secondPre (next, methodArg1, methodArg2) {
console.log(methodArg1);
// => 'altered-originalValOfMethodArg1'
...
```

#### <a name="apidoc.element.mongoose.document.prototype.unmarkModified"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>unmarkModified (path)](#apidoc.element.mongoose.document.prototype.unmarkModified)
- description and source-code
```javascript
unmarkModified = function (path) {
  this.$__.activePaths.init(path);
}
```
- example usage
```shell
...

/**
 * Clears the modified state on the specified path.
 *
 * ####Example:
 *
 *     doc.foo = 'bar';
 *     doc.unmarkModified('foo');
 *     doc.save() // changes to foo will not be persisted
 *
 * @param {String} path the path to unmark modified
 * @api public
 */

Document.prototype.unmarkModified = function(path) {
...
```

#### <a name="apidoc.element.mongoose.document.prototype.update"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>update ()](#apidoc.element.mongoose.document.prototype.update)
- description and source-code
```javascript
function update() {
  var args = utils.args(arguments);
  args.unshift({_id: this._id});
  return this.constructor.update.apply(this.constructor, args);
}
```
- example usage
```shell
...
}

/**
* Sends an update command with this document '_id' as the query selector.
*
* ####Example:
*
*     weirdCar.update({$inc: {wheels:1}}, { w: 1 }, callback);
*
* ####Valid options:
*
*  - same as in [Model.update](#model_Model.update)
*
* @see Model.update #model_Model.update
* @param {Object} doc
...
```

#### <a name="apidoc.element.mongoose.document.prototype.validate"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>validate (options, callback)](#apidoc.element.mongoose.document.prototype.validate)
- description and source-code
```javascript
validate = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }

  this.$__validate(callback || function() {});
}
```
- example usage
```shell
...
*
* ####Note:
*
* This method is called 'pre' save and if a validation rule is violated, [save](#model_Model-save) is aborted and the error is returned
 to your 'callback'.
*
* ####Example:
*
*     doc.validate(function (err) {
*       if (err) handleError(err);
*       else // validation passed
*     });
*
* @param {Object} optional options internal options
* @param {Function} callback optional callback called after validation completes, passing an error if one occurred
* @return {Promise} Promise
...
```

#### <a name="apidoc.element.mongoose.document.prototype.validateSync"></a>[function <span class="apidocSignatureSpan">mongoose.document.prototype.</span>validateSync (pathsToValidate)](#apidoc.element.mongoose.document.prototype.validateSync)
- description and source-code
```javascript
validateSync = function (pathsToValidate) {
  var _this = this;

  if (typeof pathsToValidate === 'string') {
    pathsToValidate = pathsToValidate.split(' ');
  }

  // only validate required fields when necessary
  var paths = _getPathsToValidate(this);

  if (pathsToValidate && pathsToValidate.length) {
    var tmp = [];
    for (var i = 0; i < paths.length; ++i) {
      if (pathsToValidate.indexOf(paths[i]) !== -1) {
        tmp.push(paths[i]);
      }
    }
    paths = tmp;
  }

  var validating = {};

  paths.forEach(function(path) {
    if (validating[path]) {
      return;
    }

    validating[path] = true;

    var p = _this.schema.path(path);
    if (!p) {
      return;
    }
    if (!_this.$isValid(path)) {
      return;
    }

    var val = _this.getValue(path);
    var err = p.doValidateSync(val, _this);
    if (err) {
      _this.invalidate(path, err, undefined, true);
    }
  });

  var err = _this.$__.validationError;
  _this.$__.validationError = undefined;
  _this.emit('validate', _this);
  _this.constructor.emit('validate', _this);

  if (err) {
    for (var key in err.errors) {
      // Make sure cast errors persist
      if (err.errors[key] instanceof MongooseError.CastError) {
        _this.invalidate(key, err.errors[key]);
      }
    }
  }

  return err;
}
```
- example usage
```shell
...
*
* ####Note:
*
* This method is useful if you need synchronous validation.
*
* ####Example:
*
*     var err = doc.validateSync();
*     if ( err ){
*       handleError( err );
*     } else {
*       // validation passed
*     }
*
* @param {Array|string} pathsToValidate only validate the given paths
...
```



# <a name="apidoc.module.mongoose.drivers"></a>[module mongoose.drivers](#apidoc.module.mongoose.drivers)

#### <a name="apidoc.element.mongoose.drivers.Binary"></a>[function <span class="apidocSignatureSpan">mongoose.drivers.</span>Binary (buffer, subType)](#apidoc.element.mongoose.drivers.Binary)
- description and source-code
```javascript
function Binary(buffer, subType) {
  if(!(this instanceof Binary)) return new Binary(buffer, subType);

  this._bsontype = 'Binary';

  if(buffer instanceof Number) {
    this.sub_type = buffer;
    this.position = 0;
  } else {
    this.sub_type = subType == null ? BSON_BINARY_SUBTYPE_DEFAULT : subType;
    this.position = 0;
  }

  if(buffer != null && !(buffer instanceof Number)) {
    // Only accept Buffer, Uint8Array or Arrays
    if(typeof buffer == 'string') {
      // Different ways of writing the length of the string for the different types
      if(typeof Buffer != 'undefined') {
        this.buffer = new Buffer(buffer);
      } else if(typeof Uint8Array != 'undefined' || (Object.prototype.toString.call(buffer) == '[object Array]')) {
        this.buffer = writeStringToArray(buffer);
      } else {
        throw new Error("only String, Buffer, Uint8Array or Array accepted");
      }
    } else {
      this.buffer = buffer;
    }
    this.position = buffer.length;
  } else {
    if(typeof Buffer != 'undefined') {
      this.buffer =  new Buffer(Binary.BUFFER_SIZE);
    } else if(typeof Uint8Array != 'undefined'){
      this.buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE));
    } else {
      this.buffer = new Array(Binary.BUFFER_SIZE);
    }
    // Set position to start of buffer
    this.position = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.drivers.ObjectId"></a>[function <span class="apidocSignatureSpan">mongoose.drivers.</span>ObjectId (id)](#apidoc.element.mongoose.drivers.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
...
*     .unwind('tags')
*     .exec(callback)
*
* ####Note:
*
* - The documents returned are plain javascript objects, not mongoose documents (since any shape of document can be returned).
* - Requires MongoDB >= 2.1
* - Mongoose does **not** cast pipeline stages. 'new Aggregate({ $match: { _id: '00000000000000000000000a' } });' will not work
unless '_id' is a string in the database. Use 'new Aggregate({ $match: { _id: mongoose.Types.ObjectId('00000000000000000000000a') } });'
instead.
*
* @see MongoDB http://docs.mongodb.org/manual/applications/aggregation/
* @see driver http://mongodb.github.com/node-mongodb-native/api-generated/collection.html#aggregate
* @param {Object|Array} [ops] aggregation operator(s) or operator array
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.drivers.ReadPreference"></a>[function <span class="apidocSignatureSpan">mongoose.drivers.</span>ReadPreference (pref, tags)](#apidoc.element.mongoose.drivers.ReadPreference)
- description and source-code
```javascript
function readPref(pref, tags) {
  if (Array.isArray(pref)) {
    tags = pref[1];
    pref = pref[0];
  }

  if (pref instanceof ReadPref) {
    return pref;
  }

  switch (pref) {
    case 'p':
      pref = 'primary';
      break;
    case 'pp':
      pref = 'primaryPreferred';
      break;
    case 's':
      pref = 'secondary';
      break;
    case 'sp':
      pref = 'secondaryPreferred';
      break;
    case 'n':
      pref = 'nearest';
      break;
  }

  return new ReadPref(pref, tags);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.error"></a>[module mongoose.error](#apidoc.module.mongoose.error)

#### <a name="apidoc.element.mongoose.error.error"></a>[function <span class="apidocSignatureSpan">mongoose.</span>error (msg)](#apidoc.element.mongoose.error.error)
- description and source-code
```javascript
function MongooseError(msg) {
  Error.call(this);
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.message = msg;
  this.name = 'MongooseError';
}
```
- example usage
```shell
...
if (!rgxProtocol.test(host)) {
  host = 'mongodb://' + host;
}

try {
  parsed = muri(host);
} catch (err) {
  this.error(err, callback);
  return new Promise.ES6(function(resolve, reject) {
    reject(err);
  });
}

database = parsed.db;
host = parsed.hosts[0].host || parsed.hosts[0].ipc;
...
```

#### <a name="apidoc.element.mongoose.error.CastError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>CastError (type, value, path, reason)](#apidoc.element.mongoose.error.CastError)
- description and source-code
```javascript
function CastError(type, value, path, reason) {
  var stringValue = util.inspect(value);
  stringValue = stringValue.replace(/^'/, '"').replace(/'$/, '"');
  if (stringValue.charAt(0) !== '"') {
    stringValue = '"' + stringValue + '"';
  }
  MongooseError.call(this, 'Cast to ' + type + ' failed for value ' +
    stringValue + ' at path "' + path + '"');
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.stringValue = stringValue;
  this.name = 'CastError';
  this.kind = type;
  this.value = value;
  this.path = path;
  this.reason = reason;
}
```
- example usage
```shell
...
      this.markModified(path);
      cleanModifiedSubpaths(this, path);
    } else {
      this.set(val, path, constructing);
    }
    return this;
  }
  this.invalidate(path, new MongooseError.CastError('Object', val, path));
  return this;
}

var schema;
var parts = path.split('.');

if (pathType === 'adhocOrUndefined' && strict) {
...
```

#### <a name="apidoc.element.mongoose.error.DivergentArrayError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>DivergentArrayError (paths)](#apidoc.element.mongoose.error.DivergentArrayError)
- description and source-code
```javascript
function DivergentArrayError(paths) {
  var msg = 'For your own good, using 'document.save()' to update an array '
          + 'which was selected using an $elemMatch projection OR '
          + 'populated using skip, limit, query conditions, or exclusion of '
          + 'the _id field when the operation results in a $pop or $set of '
          + 'the entire array is not supported. The following '
          + 'path(s) would have been modified unsafely:\n'
          + '  ' + paths.join('\n  ') + '\n'
          + 'Use Model.update() to update these arrays instead.';
          // TODO write up a docs page (FAQ) and link to it

  MongooseError.call(this, msg);
  Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  this.name = 'DivergentArrayError';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.error.DocumentNotFoundError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>DocumentNotFoundError (query)](#apidoc.element.mongoose.error.DocumentNotFoundError)
- description and source-code
```javascript
function DocumentNotFoundError(query) {
  MongooseError.call(this, 'No document found for query "' +
    util.inspect(query) + '"');

  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }

  this.name = 'DocumentNotFoundError';
  this.query = query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.error.MissingSchemaError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>MissingSchemaError (name)](#apidoc.element.mongoose.error.MissingSchemaError)
- description and source-code
```javascript
function MissingSchemaError(name) {
  var msg = 'Schema hasn\'t been registered for model "' + name + '".\n'
          + 'Use mongoose.model(name, schema)';
  MongooseError.call(this, msg);
  Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  this.name = 'MissingSchemaError';
}
```
- example usage
```shell
...

  if (obj._id === undefined) {
    obj._id = new ObjectId();
  }
}

if (!schema) {
  throw new MongooseError.MissingSchemaError();
}

this.$__setSchema(schema);

this.$__ = new InternalCache;
this.$__.emitter = new EventEmitter();
this.isNew = true;
...
```

#### <a name="apidoc.element.mongoose.error.OverwriteModelError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>OverwriteModelError (name)](#apidoc.element.mongoose.error.OverwriteModelError)
- description and source-code
```javascript
function OverwriteModelError(name) {
  MongooseError.call(this, 'Cannot overwrite '' + name + '' model once compiled.');
  Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  this.name = 'OverwriteModelError';
}
```
- example usage
```shell
...
  throw new Error('The 2nd parameter to 'mongoose.model()' should be a ' +
    'schema or a POJO');
}

if (this.models[name] && !collection) {
  // model exists but we are not subclassing with custom collection
  if (schema && schema.instanceOfSchema && schema !== this.models[name].schema) {
    throw new MongooseError.OverwriteModelError(name);
  }
  return this.models[name];
}

var opts = {cache: false, connection: this};
var model;
...
```

#### <a name="apidoc.element.mongoose.error.ValidationError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>ValidationError (instance)](#apidoc.element.mongoose.error.ValidationError)
- description and source-code
```javascript
function ValidationError(instance) {
  this.errors = {};
  if (instance && instance.constructor.name === 'model') {
    MongooseError.call(this, instance.constructor.modelName + ' validation failed');
  } else {
    MongooseError.call(this, 'Validation failed');
  }
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.name = 'ValidationError';
  if (instance) {
    instance.errors = this.errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.error.ValidatorError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>ValidatorError (properties)](#apidoc.element.mongoose.error.ValidatorError)
- description and source-code
```javascript
function ValidatorError(properties) {
  var msg = properties.message;
  if (!msg) {
    msg = MongooseError.messages.general.default;
  }

  var message = this.formatMessage(msg, properties);
  MongooseError.call(this, message);
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.properties = properties;
  this.name = 'ValidatorError';
  this.kind = properties.type;
  this.path = properties.path;
  this.value = properties.value;
  this.reason = properties.reason;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.error.VersionError"></a>[function <span class="apidocSignatureSpan">mongoose.error.</span>VersionError (doc)](#apidoc.element.mongoose.error.VersionError)
- description and source-code
```javascript
function VersionError(doc) {
  MongooseError.call(this, 'No matching document found for id "' + doc._id +
    '"');
  this.name = 'VersionError';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.error.prototype"></a>[module mongoose.error.prototype](#apidoc.module.mongoose.error.prototype)

#### <a name="apidoc.element.mongoose.error.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mongoose.error.prototype.</span>constructor ()](#apidoc.element.mongoose.error.prototype.constructor)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
...
}

if (obj.constructor) {
  switch (exports.getFunctionName(obj.constructor)) {
    case 'Object':
      return cloneObject(obj, options);
    case 'Date':
      return new obj.constructor(+obj);
    case 'RegExp':
      return cloneRegExp(obj);
    default:
      // ignore
      break;
  }
}
...
```



# <a name="apidoc.module.mongoose.model"></a>[module mongoose.model](#apidoc.module.mongoose.model)

#### <a name="apidoc.element.mongoose.model.model"></a>[function <span class="apidocSignatureSpan">mongoose.</span>model (doc, fields, skipId)](#apidoc.element.mongoose.model.model)
- description and source-code
```javascript
function Model(doc, fields, skipId) {
  Document.call(this, doc, fields, skipId, true);
}
```
- example usage
```shell
...
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model

Once we define a model through 'mongoose.model('ModelName', mySchema)', we can access it through the same function

'''js
var myModel = mongoose.model('ModelName');
'''

Or just do it all at once
...
```

#### <a name="apidoc.element.mongoose.model.__subclass"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>__subclass (conn, schema, collection)](#apidoc.element.mongoose.model.__subclass)
- description and source-code
```javascript
function subclass(conn, schema, collection) {
  // subclass model using this connection and collection name
  var _this = this;

  var Model = function Model(doc, fields, skipId) {
    if (!(this instanceof Model)) {
      return new Model(doc, fields, skipId);
    }
    _this.call(this, doc, fields, skipId);
  };

  Model.__proto__ = _this;
  Model.prototype.__proto__ = _this.prototype;
  Model.db = Model.prototype.db = conn;

  var s = schema && typeof schema !== 'string'
      ? schema
      : _this.prototype.schema;

  var options = s.options || {};

  if (!collection) {
    collection = _this.prototype.schema.get('collection')
        || utils.toCollectionName(_this.modelName, options);
  }

  var collectionOptions = {
    bufferCommands: s ? options.bufferCommands : true,
    capped: s && options.capped
  };

  Model.prototype.collection = conn.collection(collection, collectionOptions);
  Model.collection = Model.prototype.collection;
  Model.init();
  return Model;
}
```
- example usage
```shell
...
  return model;
}

if (this.models[name] && collection) {
  // subclassing current model with alternate collection
  model = this.models[name];
  schema = model.prototype.schema;
  var sub = model.__subclass(this, schema, collection);
  // do not cache the sub model
  return sub;
}

// lookup model in mongoose module
model = this.base.models[name];
...
```

#### <a name="apidoc.element.mongoose.model._getSchema"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>_getSchema (path)](#apidoc.element.mongoose.model._getSchema)
- description and source-code
```javascript
function _getSchema(path) {
  return this.schema._getSchema(path);
}
```
- example usage
```shell
...
    map = [],
    modelNameFromQuery = options.model && options.model.modelName || options.model,
    schema, refPath, Model, currentOptions, modelNames, modelName, discriminatorKey, modelForFindSchema;

var originalOptions = utils.clone(options);
var isVirtual = false;

schema = model._getSchema(options.path);
var isUnderneathDocArray = schema && schema.$isUnderneathDocArray;
if (isUnderneathDocArray &&
    originalOptions &&
    originalOptions.options &&
    originalOptions.options.sort) {
  return new Error('Cannot populate with 'sort' on path ' + options.path +
    ' because it is a subproperty of a document array');
...
```

#### <a name="apidoc.element.mongoose.model.addListener"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>addListener (type, listener)](#apidoc.element.mongoose.model.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.aggregate"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>aggregate ()](#apidoc.element.mongoose.model.aggregate)
- description and source-code
```javascript
function aggregate() {
  var args = [].slice.call(arguments),
      aggregate,
      callback;

  if (typeof args[args.length - 1] === 'function') {
    callback = args.pop();
  }

  if (args.length === 1 && util.isArray(args[0])) {
    aggregate = new Aggregate(args[0]);
  } else {
    aggregate = new Aggregate(args);
  }

  aggregate.model(this);

  if (typeof callback === 'undefined') {
    return aggregate;
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  aggregate.exec(callback);
}
```
- example usage
```shell
...
* ####Example:
*
*     new Aggregate();
*     new Aggregate({ $project: { a: 1, b: 1 } });
*     new Aggregate({ $project: { a: 1, b: 1 } }, { $skip: 5 });
*     new Aggregate([{ $project: { a: 1, b: 1 } }, { $skip: 5 }]);
*
* Returned when calling Model.aggregate().
*
* ####Example:
*
*     Model
*     .aggregate({ $match: { age: { $gte: 21 }}})
*     .unwind('tags')
*     .exec(callback)
...
```

#### <a name="apidoc.element.mongoose.model.bulkWrite"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>bulkWrite (ops, options, callback)](#apidoc.element.mongoose.model.bulkWrite)
- description and source-code
```javascript
bulkWrite = function (ops, options, callback) {
  var Promise = PromiseProvider.get();
  var _this = this;
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }
  options = options || {};

  var validations = ops.map(function(op) {
    if (op['insertOne']) {
      return function(callback) {
        op['insertOne']['document'] = new _this(op['insertOne']['document']);
        op['insertOne']['document'].validate({ __noPromise: true }, function(error) {
          if (error) {
            return callback(error);
          }
          callback(null);
        });
      };
    } else if (op['updateOne']) {
      return function(callback) {
        try {
          op['updateOne']['filter'] = cast(_this.schema,
            op['updateOne']['filter']);
          op['updateOne']['update'] = castUpdate(_this.schema,
            op['updateOne']['update'], _this.schema.options.strict);
        } catch (error) {
          return callback(error);
        }

        callback(null);
      };
    } else if (op['updateMany']) {
      return function(callback) {
        try {
          op['updateMany']['filter'] = cast(_this.schema,
            op['updateMany']['filter']);
          op['updateMany']['update'] = castUpdate(_this.schema, op['updateMany']['filter'], {
            strict: _this.schema.options.strict,
            overwrite: false
          });
        } catch (error) {
          return callback(error);
        }

        callback(null);
      };
    } else if (op['replaceOne']) {
      return function(callback) {
        try {
          op['replaceOne']['filter'] = cast(_this.schema,
            op['replaceOne']['filter']);
        } catch (error) {
          return callback(error);
        }

        // set 'skipId', otherwise we get "_id field cannot be changed"
        op['replaceOne']['replacement'] =
          new _this(op['replaceOne']['replacement'], null, true);
        op['replaceOne']['replacement'].validate({ __noPromise: true }, function(error) {
          if (error) {
            return callback(error);
          }
          callback(null);
        });
      };
    } else if (op['deleteOne']) {
      return function(callback) {
        try {
          op['deleteOne']['filter'] = cast(_this.schema,
            op['deleteOne']['filter']);
        } catch (error) {
          return callback(error);
        }

        callback(null);
      };
    } else if (op['deleteMany']) {
      return function(callback) {
        try {
          op['deleteMany']['filter'] = cast(_this.schema,
            op['deleteMany']['filter']);
        } catch (error) {
          return callback(error);
        }

        callback(null);
      };
    } else {
      return function(callback) {
        callback(new Error('Invalid op passed to 'bulkWrite()''));
      };
    }
  });

  var promise = new Promise.ES6(function(resolve, reject) {
    parallel(validations, function(error) {
      if (error) {
        callback && callback(error);
        return reject(error);
      }

      _this.collection.bulkWrite(ops, options, function(error, res) {
        if (error) {
          callback && callback(error);
          return reject(error);
        }

        callback && callback(null, res);
        resolve(res);
      });
    });
  });

  return promise;
}
```
- example usage
```shell
...
*
* Mongoose will perform casting on all operations you provide.
*
* This function does **not** trigger any middleware.
*
* ####Example:
*
*     Character.bulkWrite([
*       {
*         insertOne: {
*           document: {
*             name: 'Eddard Stark',
*             title: 'Warden of the North'
*           }
*         }
...
```

#### <a name="apidoc.element.mongoose.model.compile"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>compile (name, schema, collectionName, connection, base)](#apidoc.element.mongoose.model.compile)
- description and source-code
```javascript
function compile(name, schema, collectionName, connection, base) {
  var versioningEnabled = schema.options.versionKey !== false;

  if (versioningEnabled && !schema.paths[schema.options.versionKey]) {
    // add versioning to top level documents only
    var o = {};
    o[schema.options.versionKey] = Number;
    schema.add(o);
  }

  var model;
  if (typeof name === 'function' && name.prototype instanceof Model) {
    model = name;
    name = model.name;
    schema.loadClass(model, true);
    model.prototype.$isMongooseModelPrototype = true;
  } else {
    // generate new class
    model = function model(doc, fields, skipId) {
      if (!(this instanceof model)) {
        return new model(doc, fields, skipId);
      }
      Model.call(this, doc, fields, skipId);
    };
  }

  model.hooks = schema.s.hooks.clone();
  model.base = base;
  model.modelName = name;
  if (!(model.prototype instanceof Model)) {
    model.__proto__ = Model;
    model.prototype.__proto__ = Model.prototype;
  }
  model.model = Model.prototype.model;
  model.db = model.prototype.db = connection;
  model.discriminators = model.prototype.discriminators = undefined;

  model.prototype.$__setSchema(schema);

  var collectionOptions = {
    bufferCommands: schema.options.bufferCommands,
    capped: schema.options.capped
  };

  model.prototype.collection = connection.collection(
      collectionName
      , collectionOptions
  );

  // apply methods and statics
  applyMethods(model, schema);
  applyStatics(model, schema);
  applyHooks(model, schema);

  model.schema = model.prototype.schema;
  model.collection = model.prototype.collection;

  // Create custom query constructor
  model.Query = function() {
    Query.apply(this, arguments);
    this.options.retainKeyOrder = model.schema.options.retainKeyOrder;
  };
  model.Query.prototype = Object.create(Query.prototype);
  model.Query.base = Query.base;
  applyQueryMethods(model, schema.query);

  var kareemOptions = { useErrorHandlers: true };
  model.$__insertMany = model.hooks.createWrapper('insertMany',
    model.insertMany, model, kareemOptions);
  model.insertMany = function(arr, options, callback) {
    var Promise = PromiseProvider.get();
    if (typeof options === 'function') {
      callback = options;
      options = null;
    }
    return new Promise.ES6(function(resolve, reject) {
      model.$__insertMany(arr, options, function(error, result) {
        if (error) {
          callback && callback(error);
          return reject(error);
        }
        callback && callback(null, result);
        resolve(result);
      });
    });
  };

  return model;
}
```
- example usage
```shell
...
callback && callback(err);
reject(err);
return;
      }

      if (ret.findOne && ret.mapReduce) {
// returned a collection, convert to Model
var model = Model.compile(
    '_mapreduce_' + ret.collectionName
    , Model.mapReduce.schema
    , ret.collectionName
    , _this.db
    , _this.base);

model._mapreduce = true;
...
```

#### <a name="apidoc.element.mongoose.model.count"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>count (conditions, callback)](#apidoc.element.mongoose.model.count)
- description and source-code
```javascript
function count(conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }

  // get the mongodb collection object
  var mq = new this.Query({}, {}, this, this.collection);

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.count(conditions, callback);
}
```
- example usage
```shell
...
};

/**
* Counts number of matching documents in a database collection.
*
* ####Example:
*
*     Adventure.count({ type: 'jungle' }, function (err, count) {
*       if (err) ..
*       console.log('there are %d jungle adventures', count);
*     });
*
* @param {Object} conditions
* @param {Function} [callback]
* @return {Query}
...
```

#### <a name="apidoc.element.mongoose.model.create"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>create (doc, callback)](#apidoc.element.mongoose.model.create)
- description and source-code
```javascript
function create(doc, callback) {
  var args;
  var cb;
  var discriminatorKey = this.schema.options.discriminatorKey;

  if (Array.isArray(doc)) {
    args = doc;
    cb = callback;
  } else {
    var last = arguments[arguments.length - 1];
    // Handle falsy callbacks re: #5061
    if (typeof last === 'function' || !last) {
      cb = last;
      args = utils.args(arguments, 0, arguments.length - 1);
    } else {
      args = utils.args(arguments);
    }
  }

  var Promise = PromiseProvider.get();
  var _this = this;
  if (cb) {
    cb = this.$wrapCallback(cb);
  }

  var promise = new Promise.ES6(function(resolve, reject) {
    if (args.length === 0) {
      setImmediate(function() {
        cb && cb(null);
        resolve(null);
      });
      return;
    }

    var toExecute = [];
    args.forEach(function(doc) {
      toExecute.push(function(callback) {
        var Model = _this.discriminators && doc[discriminatorKey] ?
          _this.discriminators[doc[discriminatorKey]] :
          _this;
        var toSave = doc instanceof Model ? doc : new Model(doc);
        var callbackWrapper = function(error, doc) {
          if (error) {
            return callback(error);
          }
          callback(null, doc);
        };

        // Hack to avoid getting a promise because of
        // $__registerHooksFromSchema
        if (toSave.$__original_save) {
          toSave.$__original_save({ __noPromise: true }, callbackWrapper);
        } else {
          toSave.save({ __noPromise: true }, callbackWrapper);
        }
      });
    });

    parallel(toExecute, function(error, savedDocs) {
      if (error) {
        if (cb) {
          cb(error);
        } else {
          reject(error);
        }
        return;
      }

      if (doc instanceof Array) {
        resolve(savedDocs);
        cb && cb.call(_this, null, savedDocs);
      } else {
        resolve.apply(promise, savedDocs);
        if (cb) {
          savedDocs.unshift(null);
          cb.apply(_this, savedDocs);
        }
      }
    });
  });

  return promise;
}
```
- example usage
```shell
...
  }
}

/*!
 * Inherit from the NodeJS document
 */

Document.prototype = Object.create(NodeJSDocument.prototype);
Document.prototype.constructor = Document;

/*!
 * Browser doc exposes the event emitter API
 */

Document.$emitter = new EventEmitter();
...
```

#### <a name="apidoc.element.mongoose.model.deleteMany"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>deleteMany (conditions, callback)](#apidoc.element.mongoose.model.deleteMany)
- description and source-code
```javascript
function deleteMany(conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }

  // get the mongodb collection object
  var mq = new this.Query(conditions, {}, this, this.collection);

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.deleteMany(callback);
}
```
- example usage
```shell
...
/**
* Deletes the first document that matches 'conditions' from the collection.
* Behaves like 'remove()', but deletes all documents that match 'conditions'
* regardless of the 'justOne' option.
*
* ####Example:
*
*     Character.deleteMany({ name: /Stark/, age: { $gte: 18 } }, function (err) {});
*
* ####Note:
*
* Like 'Model.remove()', this function does **not** trigger 'pre('remove')' or 'post('remove')' hooks.
*
* @param {Object} conditions
* @param {Function} [callback]
...
```

#### <a name="apidoc.element.mongoose.model.deleteOne"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>deleteOne (conditions, callback)](#apidoc.element.mongoose.model.deleteOne)
- description and source-code
```javascript
function deleteOne(conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }

  // get the mongodb collection object
  var mq = new this.Query(conditions, {}, this, this.collection);

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.deleteOne(callback);
}
```
- example usage
```shell
...
/**
* Deletes the first document that matches 'conditions' from the collection.
* Behaves like 'remove()', but deletes at most one document regardless of the
* 'justOne' option.
*
* ####Example:
*
*     Character.deleteOne({ name: 'Eddard Stark' }, function (err) {});
*
* ####Note:
*
* Like 'Model.remove()', this function does **not** trigger 'pre('remove')' or 'post('remove')' hooks.
*
* @param {Object} conditions
* @param {Function} [callback]
...
```

#### <a name="apidoc.element.mongoose.model.discriminator"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>discriminator (name, schema)](#apidoc.element.mongoose.model.discriminator)
- description and source-code
```javascript
discriminator = function (name, schema) {
  schema = discriminator(this, name, schema);
  if (this.db.models[name]) {
    throw new OverwriteModelError(name);
  }

  var _name;
  if (typeof name === 'function') {
    _name = utils.getFunctionName(name);
  } else {
    _name = name;
  }

  schema.$isRootDiscriminator = true;

  this.discriminators[_name] = this.db.model(name, schema, this.collection.name);
  var d = this.discriminators[_name];
  d.prototype.__proto__ = this.prototype;
  Object.defineProperty(d, 'baseModelName', {
    value: this.modelName,
    configurable: true,
    writable: false
  });

  // apply methods and statics
  applyMethods(d, schema);
  applyStatics(d, schema);

  return d;
}
```
- example usage
```shell
...
 *     }
 *     util.inherits(BaseSchema, Schema);
 *
 *     var PersonSchema = new BaseSchema();
 *     var BossSchema = new BaseSchema({ department: String });
 *
 *     var Person = mongoose.model('Person', PersonSchema);
 *     var Boss = Person.discriminator('Boss', BossSchema);
 *
 * @param {String} name   discriminator model name
 * @param {Schema} schema discriminator model schema
 * @api public
 */

Model.discriminator = function(name, schema) {
...
```

#### <a name="apidoc.element.mongoose.model.distinct"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>distinct (field, conditions, callback)](#apidoc.element.mongoose.model.distinct)
- description and source-code
```javascript
function distinct(field, conditions, callback) {
  // get the mongodb collection object
  var mq = new this.Query({}, {}, this, this.collection);

  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.distinct(field, conditions, callback);
}
```
- example usage
```shell
...
/**
* Creates a Query for a 'distinct' operation.
*
* Passing a 'callback' immediately executes the query.
*
* ####Example
*
*     Link.distinct('url', { clicks: {$gt: 100}}, function (err, result) {
*       if (err) return handleError(err);
*
*       assert(Array.isArray(result));
*       console.log('unique urls with more than 100 clicks', result);
*     })
*
*     var query = Link.distinct('url');
...
```

#### <a name="apidoc.element.mongoose.model.emit"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>emit (type)](#apidoc.element.mongoose.model.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
You can intercept method arguments via middleware.

For example, this would allow you to broadcast changes about your Documents every time someone 'set's a path in your Document to
 a new value:

'''js
schema.pre('set', function (next, path, val, typel) {
  // 'this' is the current Document
  this.emit('set', path, val);

  // Pass control to the next pre
  next();
});
'''

Moreover, you can mutate the incoming 'method' arguments so that subsequent middleware see different values for those arguments.
To do so, just pass the new values to 'next':
...
```

#### <a name="apidoc.element.mongoose.model.ensureIndexes"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>ensureIndexes (options, callback)](#apidoc.element.mongoose.model.ensureIndexes)
- description and source-code
```javascript
function ensureIndexes(options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }

  if (options && options.__noPromise) {
    _ensureIndexes(this, options, callback);
    return;
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  var _this = this;
  var Promise = PromiseProvider.get();
  return new Promise.ES6(function(resolve, reject) {
    _ensureIndexes(_this, options || {}, function(error) {
      if (error) {
        callback && callback(error);
        reject(error);
      }
      callback && callback();
      resolve();
    });
  });
}
```
- example usage
```shell
...
*
* @api private
*/

Model.init = function init() {
 if ((this.schema.options.autoIndex) ||
     (this.schema.options.autoIndex === null && this.db.config.autoIndex)) {
   this.ensureIndexes({ __noPromise: true, _automatic: true });
 }

 this.schema.emit('init', this);
};

/**
* Sends 'ensureIndex' commands to mongo for each index declared in the schema.
...
```

#### <a name="apidoc.element.mongoose.model.eventNames"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>eventNames ()](#apidoc.element.mongoose.model.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.find"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>find (conditions, projection, options, callback)](#apidoc.element.mongoose.model.find)
- description and source-code
```javascript
function find(conditions, projection, options, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
    projection = null;
    options = null;
  } else if (typeof projection === 'function') {
    callback = projection;
    projection = null;
    options = null;
  } else if (typeof options === 'function') {
    callback = options;
    options = null;
  }

  var mq = new this.Query({}, {}, this, this.collection);
  mq.select(projection);
  mq.setOptions(options);
  if (this.schema.discriminatorMapping && mq.selectedInclusively()) {
    mq.select(this.schema.options.discriminatorKey);
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.find(conditions, callback);
}
```
- example usage
```shell
...
  //
});
'''

Or we can find documents from the same collection

'''js
MyModel.find({}, function (err, docs) {
  // docs.forEach
});
'''

You can also 'findOne', 'findById', 'update', etc. For more details check out [the docs](http://mongoosejs.com/docs/queries.html
).

**Important!** If you opened a separate connection using 'mongoose.createConnection()' but attempt to access the model through '
mongoose.model('ModelName')' it will not work as expected since it is not hooked up to an active db connection. In this case access
 your model through the connection you created:
...
```

#### <a name="apidoc.element.mongoose.model.findById"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findById (id, projection, options, callback)](#apidoc.element.mongoose.model.findById)
- description and source-code
```javascript
function findById(id, projection, options, callback) {
  if (typeof id === 'undefined') {
    id = null;
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return this.findOne({_id: id}, projection, options, callback);
}
```
- example usage
```shell
...
  if (!err) console.log('Success!');
});
'''

The same goes for removing them:

'''js
BlogPost.findById(myId, function (err, post) {
  if (!err) {
    post.comments[0].remove();
    post.save(function (err) {
      // do something
    });
  }
});
...
```

#### <a name="apidoc.element.mongoose.model.findByIdAndRemove"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findByIdAndRemove (id, options, callback)](#apidoc.element.mongoose.model.findByIdAndRemove)
- description and source-code
```javascript
findByIdAndRemove = function (id, options, callback) {
  if (arguments.length === 1 && typeof id === 'function') {
    var msg = 'Model.findByIdAndRemove(): First argument must not be a function.\n\n'
        + '  ' + this.modelName + '.findByIdAndRemove(id, callback)\n'
        + '  ' + this.modelName + '.findByIdAndRemove(id)\n'
        + '  ' + this.modelName + '.findByIdAndRemove()\n';
    throw new TypeError(msg);
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return this.findOneAndRemove({_id: id}, options, callback);
}
```
- example usage
```shell
...
* ####Options:
*
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'select': sets the document fields to return
*
* ####Examples:
*
*     A.findByIdAndRemove(id, options, callback) // executes
*     A.findByIdAndRemove(id, options)  // return Query
*     A.findByIdAndRemove(id, callback) // executes
*     A.findByIdAndRemove(id) // returns Query
*     A.findByIdAndRemove()           // returns Query
*
* @param {Object|Number|String} id value of '_id' to query by
* @param {Object} [options]
...
```

#### <a name="apidoc.element.mongoose.model.findByIdAndUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findByIdAndUpdate (id, update, options, callback)](#apidoc.element.mongoose.model.findByIdAndUpdate)
- description and source-code
```javascript
findByIdAndUpdate = function (id, update, options, callback) {
  if (callback) {
    callback = this.$wrapCallback(callback);
  }
  if (arguments.length === 1) {
    if (typeof id === 'function') {
      var msg = 'Model.findByIdAndUpdate(): First argument must not be a function.\n\n'
          + '  ' + this.modelName + '.findByIdAndUpdate(id, callback)\n'
          + '  ' + this.modelName + '.findByIdAndUpdate(id)\n'
          + '  ' + this.modelName + '.findByIdAndUpdate()\n';
      throw new TypeError(msg);
    }
    return this.findOneAndUpdate({_id: id}, undefined);
  }

  // if a model is passed in instead of an id
  if (id instanceof Document) {
    id = id._id;
  }

  return this.findOneAndUpdate.call(this, {_id: id}, update, options, callback);
}
```
- example usage
```shell
...
* - 'runValidators': if true, runs [update validators](/docs/validation.html#update-validators) on this command. Update validators
 validate the update operation against the model's schema.
* - 'setDefaultsOnInsert': if this and 'upsert' are true, mongoose will apply the [defaults](http://mongoosejs.com/docs/defaults
.html) specified in the model's schema if a new document is created. This option only works on MongoDB >= 2.4 because it relies
on [MongoDB's '$setOnInsert' operator](https://docs.mongodb.org/v2.4/reference/operator/update/setOnInsert/).
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'select': sets the document fields to return
*
* ####Examples:
*
*     A.findByIdAndUpdate(id, update, options, callback) // executes
*     A.findByIdAndUpdate(id, update, options)  // returns Query
*     A.findByIdAndUpdate(id, update, callback) // executes
*     A.findByIdAndUpdate(id, update)           // returns Query
*     A.findByIdAndUpdate()                     // returns Query
*
* ####Note:
*
...
```

#### <a name="apidoc.element.mongoose.model.findOne"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findOne (conditions, projection, options, callback)](#apidoc.element.mongoose.model.findOne)
- description and source-code
```javascript
function findOne(conditions, projection, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  } else if (typeof projection === 'function') {
    callback = projection;
    projection = null;
    options = null;
  } else if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
    projection = null;
    options = null;
  }

  // get the mongodb collection object
  var mq = new this.Query({}, {}, this, this.collection);
  mq.select(projection);
  mq.setOptions(options);
  if (this.schema.discriminatorMapping && mq.selectedInclusively()) {
    mq.select(this.schema.options.discriminatorKey);
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.findOne(conditions, callback);
}
```
- example usage
```shell
...
};

/**
* Checks if 'path' was selected in the source query which initialized this document.
*
* ####Example
*
*     Thing.findOne().select('name').exec(function (err, doc) {
*        doc.isSelected('name') // true
*        doc.isSelected('age')  // false
*     })
*
* @param {String} path
* @return {Boolean}
* @api public
...
```

#### <a name="apidoc.element.mongoose.model.findOneAndRemove"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findOneAndRemove (conditions, options, callback)](#apidoc.element.mongoose.model.findOneAndRemove)
- description and source-code
```javascript
findOneAndRemove = function (conditions, options, callback) {
  if (arguments.length === 1 && typeof conditions === 'function') {
    var msg = 'Model.findOneAndRemove(): First argument must not be a function.\n\n'
        + '  ' + this.modelName + '.findOneAndRemove(conditions, callback)\n'
        + '  ' + this.modelName + '.findOneAndRemove(conditions)\n'
        + '  ' + this.modelName + '.findOneAndRemove()\n';
    throw new TypeError(msg);
  }

  if (typeof options === 'function') {
    callback = options;
    options = undefined;
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  var fields;
  if (options) {
    fields = options.select;
    options.select = undefined;
  }

  var mq = new this.Query({}, {}, this, this.collection);
  mq.select(fields);

  return mq.findOneAndRemove(conditions, options, callback);
}
```
- example usage
```shell
...
*
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'maxTimeMS': puts a time limit on the query - requires mongodb >= 2.6.0
* - 'select': sets the document fields to return
*
* ####Examples:
*
*     A.findOneAndRemove(conditions, options, callback) // executes
*     A.findOneAndRemove(conditions, options)  // return Query
*     A.findOneAndRemove(conditions, callback) // executes
*     A.findOneAndRemove(conditions) // returns Query
*     A.findOneAndRemove()           // returns Query
*
* Values are cast to their appropriate types when using the findAndModify helpers.
* However, the below are never executed.
...
```

#### <a name="apidoc.element.mongoose.model.findOneAndUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>findOneAndUpdate (conditions, update, options, callback)](#apidoc.element.mongoose.model.findOneAndUpdate)
- description and source-code
```javascript
findOneAndUpdate = function (conditions, update, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  } else if (arguments.length === 1) {
    if (typeof conditions === 'function') {
      var msg = 'Model.findOneAndUpdate(): First argument must not be a function.\n\n'
          + '  ' + this.modelName + '.findOneAndUpdate(conditions, update, options, callback)\n'
          + '  ' + this.modelName + '.findOneAndUpdate(conditions, update, options)\n'
          + '  ' + this.modelName + '.findOneAndUpdate(conditions, update)\n'
          + '  ' + this.modelName + '.findOneAndUpdate(update)\n'
          + '  ' + this.modelName + '.findOneAndUpdate()\n';
      throw new TypeError(msg);
    }
    update = conditions;
    conditions = undefined;
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  var fields;
  if (options && options.fields) {
    fields = options.fields;
  }

  update = utils.clone(update, {depopulate: 1, _isNested: true});
  if (this.schema.options.versionKey && options && options.upsert) {
    if (!update.$setOnInsert) {
      update.$setOnInsert = {};
    }
    update.$setOnInsert[this.schema.options.versionKey] = 0;
  }

  var mq = new this.Query({}, {}, this, this.collection);
  mq.select(fields);

  return mq.findOneAndUpdate(conditions, update, options, callback);
}
```
- example usage
```shell
...
*
* Finds a matching document, updates it according to the 'update' arg, passing any 'options', and returns the found document (if
 any) to the callback. The query executes immediately if 'callback' is passed else a Query object is returned.
*
* ####Options:
*
* - 'new': bool - if true, return the modified document rather than the original. defaults to false (changed in 4.0)
* - 'upsert': bool - creates the object if it doesn't exist. defaults to false.
* - 'fields': {Object|String} - Field selection. Equivalent to '.select(fields).findOneAndUpdate()'
* - 'maxTimeMS': puts a time limit on the query - requires mongodb >= 2.6.0
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'runValidators': if true, runs [update validators](/docs/validation.html#update-validators) on this command. Update validators
 validate the update operation against the model's schema.
* - 'setDefaultsOnInsert': if this and 'upsert' are true, mongoose will apply the [defaults](http://mongoosejs.com/docs/defaults
.html) specified in the model's schema if a new document is created. This option only works on MongoDB >= 2.4 because it relies
on [MongoDB's '$setOnInsert' operator](https://docs.mongodb.org/v2.4/reference/operator/update/setOnInsert/).
* - 'passRawResult': if true, passes the [raw result from the MongoDB driver as the third callback parameter](http://mongodb.github
.io/node-mongodb-native/2.0/api/Collection.html#findAndModify)
*
*
...
```

#### <a name="apidoc.element.mongoose.model.geoNear"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>geoNear (near, options, callback)](#apidoc.element.mongoose.model.geoNear)
- description and source-code
```javascript
geoNear = function (near, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  var _this = this;
  var Promise = PromiseProvider.get();
  if (!near) {
    return new Promise.ES6(function(resolve, reject) {
      var error = new Error('Must pass a near option to geoNear');
      reject(error);
      callback && callback(error);
    });
  }

  var x, y;

  return new Promise.ES6(function(resolve, reject) {
    var handler = function(err, res) {
      if (err) {
        reject(err);
        callback && callback(err);
        return;
      }
      if (options.lean) {
        resolve(res.results, res.stats);
        callback && callback(null, res.results, res.stats);
        return;
      }

      var count = res.results.length;
      // if there are no results, fulfill the promise now
      if (count === 0) {
        resolve(res.results, res.stats);
        callback && callback(null, res.results, res.stats);
        return;
      }

      var errSeen = false;

      function init(err) {
        if (err && !errSeen) {
          errSeen = true;
          reject(err);
          callback && callback(err);
          return;
        }
        if (--count <= 0) {
          resolve(res.results, res.stats);
          callback && callback(null, res.results, res.stats);
        }
      }

      for (var i = 0; i < res.results.length; i++) {
        var temp = res.results[i].obj;
        res.results[i].obj = new _this();
        res.results[i].obj.init(temp, init);
      }
    };

    if (Array.isArray(near)) {
      if (near.length !== 2) {
        var error = new Error('If using legacy coordinates, must be an array ' +
            'of size 2 for geoNear');
        reject(error);
        callback && callback(error);
        return;
      }
      x = near[0];
      y = near[1];
      _this.collection.geoNear(x, y, options, handler);
    } else {
      if (near.type !== 'Point' || !Array.isArray(near.coordinates)) {
        error = new Error('Must pass either a legacy coordinate array or ' +
            'GeoJSON Point to geoNear');
        reject(error);
        callback && callback(error);
        return;
      }

      _this.collection.geoNear(near, options, handler);
    }
  });
}
```
- example usage
```shell
...
* ####Options:
* - 'lean' {Boolean} return the raw object
* - All options supported by the driver are also supported
*
* ####Example:
*
*     // Legacy point
*     Model.geoNear([1,3], { maxDistance : 5, spherical : true }, function(err, results, stats) {
*        console.log(results);
*     });
*
*     // geoJson
*     var point = { type : "Point", coordinates : [9,9] };
*     Model.geoNear(point, { maxDistance : 5, spherical : true }, function(err, results, stats) {
*        console.log(results);
...
```

#### <a name="apidoc.element.mongoose.model.geoSearch"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>geoSearch (conditions, options, callback)](#apidoc.element.mongoose.model.geoSearch)
- description and source-code
```javascript
geoSearch = function (conditions, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  var _this = this;
  var Promise = PromiseProvider.get();
  return new Promise.ES6(function(resolve, reject) {
    var error;
    if (conditions === undefined || !utils.isObject(conditions)) {
      error = new Error('Must pass conditions to geoSearch');
    } else if (!options.near) {
      error = new Error('Must specify the near option in geoSearch');
    } else if (!Array.isArray(options.near)) {
      error = new Error('near option must be an array [x, y]');
    }

    if (error) {
      callback && callback(error);
      reject(error);
      return;
    }

    // send the conditions in the options object
    options.search = conditions;

    _this.collection.geoHaystackSearch(options.near[0], options.near[1], options, function(err, res) {
      // have to deal with driver problem. Should be fixed in a soon-ish release
      // (7/8/2013)
      if (err) {
        callback && callback(err);
        reject(err);
        return;
      }

      var count = res.results.length;
      if (options.lean || count === 0) {
        callback && callback(null, res.results, res.stats);
        resolve(res.results, res.stats);
        return;
      }

      var errSeen = false;

      function init(err) {
        if (err && !errSeen) {
          callback && callback(err);
          reject(err);
          return;
        }

        if (!--count && !errSeen) {
          callback && callback(null, res.results, res.stats);
          resolve(res.results, res.stats);
        }
      }

      for (var i = 0; i < res.results.length; i++) {
        var temp = res.results[i];
        res.results[i] = new _this();
        res.results[i].init(temp, {}, init);
      }
    });
  });
}
```
- example usage
```shell
...

/**
* Implements '$geoSearch' functionality for Mongoose
*
* ####Example:
*
*     var options = { near: [10, 10], maxDistance: 5 };
*     Locations.geoSearch({ type : "house" }, options, function(err, res) {
*       console.log(res);
*     });
*
* ####Options:
* - 'near' {Array} x,y point to search for
* - 'maxDistance' {Number} the maximum distance from the point near that a result can be
* - 'limit' {Number} The maximum number of results to return
...
```

#### <a name="apidoc.element.mongoose.model.getMaxListeners"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>getMaxListeners ()](#apidoc.element.mongoose.model.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.hydrate"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>hydrate (obj)](#apidoc.element.mongoose.model.hydrate)
- description and source-code
```javascript
hydrate = function (obj) {
  var model = require('./queryhelpers').createModel(this, obj);
  model.init(obj);
  return model;
}
```
- example usage
```shell
...
/**
 * Shortcut for creating a new Document from existing raw data, pre-saved in the DB.
 * The document returned has no paths marked as modified initially.
 *
 * ####Example:
 *
 *     // hydrate previous data into a Mongoose document
 *     var mongooseCandy = Candy.hydrate({ _id: '54108337212ffb6d459f854c', type: 'jelly bean' });
 *
 * @param {Object} obj
 * @return {Document}
 * @api public
 */

Model.hydrate = function(obj) {
...
```

#### <a name="apidoc.element.mongoose.model.init"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>init ()](#apidoc.element.mongoose.model.init)
- description and source-code
```javascript
function init() {
  if ((this.schema.options.autoIndex) ||
      (this.schema.options.autoIndex === null && this.db.config.autoIndex)) {
    this.ensureIndexes({ __noPromise: true, _automatic: true });
  }

  this.schema.emit('init', this);
}
```
- example usage
```shell
...
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);

if (!skipInit && obj) {
  this.init(obj);
}

this.$__registerHooksFromSchema();

// apply methods
for (var m in schema.methods) {
  this[m] = schema.methods[m];
...
```

#### <a name="apidoc.element.mongoose.model.insertMany"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>insertMany (arr, options, callback)](#apidoc.element.mongoose.model.insertMany)
- description and source-code
```javascript
insertMany = function (arr, options, callback) {
  var _this = this;
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  if (!Array.isArray(arr)) {
    arr = [arr];
  }

  var toExecute = [];
  arr.forEach(function(doc) {
    toExecute.push(function(callback) {
      doc = new _this(doc);
      doc.validate({ __noPromise: true }, function(error) {
        if (error) {
          // Option 'ordered' signals that insert should be continued after reaching
          // a failing insert. Therefore we delegate "null", meaning the validation
          // failed. It's up to the next function to filter out all failed models
          if (options != null && typeof options === 'object' && options['ordered'] === false) {
            return callback(null, null);
          }
          return callback(error);
        }
        callback(null, doc);
      });
    });
  });

  parallel(toExecute, function(error, docs) {
    if (error) {
      callback && callback(error);
      return;
    }
    // We filter all failed pre-validations by removing nulls
    var docAttributes = docs.filter(function(doc) {
      return doc != null;
    });
    // Quickly escape while there aren't any valid docAttributes
    if (docAttributes.length < 1) {
      callback && callback(null, []);
      return;
    }
    var docObjects = docAttributes.map(function(doc) {
      if (doc.schema.options.versionKey) {
        doc[doc.schema.options.versionKey] = 0;
      }
      if (doc.initializeTimestamps) {
        return doc.initializeTimestamps().toObject(POJO_TO_OBJECT_OPTIONS);
      }
      return doc.toObject(POJO_TO_OBJECT_OPTIONS);
    });
    _this.collection.insertMany(docObjects, options, function(error) {
      if (error) {
        callback && callback(error);
        return;
      }
      for (var i = 0; i < docAttributes.length; ++i) {
        docAttributes[i].isNew = false;
        docAttributes[i].emit('isNew', false);
        docAttributes[i].constructor.emit('isNew', false);
      }
      callback && callback(null, docAttributes);
    });
  });
}
```
- example usage
```shell
...
* document.
*
* This function does **not** trigger save middleware.
*
* ####Example:
*
*     var arr = [{ name: 'Star Wars' }, { name: 'The Empire Strikes Back' }];
*     Movies.insertMany(arr, function(error, docs) {});
*
* @param {Array|Object|*} doc(s)
* @param {Object} [options] see the [mongodb driver options](http://mongodb.github.io/node-mongodb-native/2.2/api/Collection.html
#insertMany)
* @param {Function} [callback] callback
* @return {Promise}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.model.listenerCount"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>listenerCount (type)](#apidoc.element.mongoose.model.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.listeners"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>listeners (type)](#apidoc.element.mongoose.model.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
...
      doc[pair[0]].apply(doc, pair[1]);
    }
  }
}

Document.prototype.$__handleReject = function handleReject(err) {
  // emit on the Model if listening
  if (this.listeners('error').length) {
    this.emit('error', err);
  } else if (this.constructor.listeners && this.constructor.listeners('error').length) {
    this.constructor.emit('error', err);
  } else if (this.listeners && this.listeners('error').length) {
    this.emit('error', err);
  }
};
...
```

#### <a name="apidoc.element.mongoose.model.mapReduce"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>mapReduce (o, callback)](#apidoc.element.mongoose.model.mapReduce)
- description and source-code
```javascript
function mapReduce(o, callback) {
  var _this = this;
  if (callback) {
    callback = this.$wrapCallback(callback);
  }
  var Promise = PromiseProvider.get();
  return new Promise.ES6(function(resolve, reject) {
    if (!Model.mapReduce.schema) {
      var opts = {noId: true, noVirtualId: true, strict: false};
      Model.mapReduce.schema = new Schema({}, opts);
    }

    if (!o.out) o.out = {inline: 1};
    if (o.verbose !== false) o.verbose = true;

    o.map = String(o.map);
    o.reduce = String(o.reduce);

    if (o.query) {
      var q = new _this.Query(o.query);
      q.cast(_this);
      o.query = q._conditions;
      q = undefined;
    }

    _this.collection.mapReduce(null, null, o, function(err, ret, stats) {
      if (err) {
        callback && callback(err);
        reject(err);
        return;
      }

      if (ret.findOne && ret.mapReduce) {
        // returned a collection, convert to Model
        var model = Model.compile(
            '_mapreduce_' + ret.collectionName
            , Model.mapReduce.schema
            , ret.collectionName
            , _this.db
            , _this.base);

        model._mapreduce = true;

        callback && callback(null, model, stats);
        return resolve(model, stats);
      }

      callback && callback(null, ret, stats);
      resolve(ret, stats);
    });
  });
}
```
- example usage
```shell
...
* 'o' is an object specifying all mapReduce options as well as the map and reduce functions. All options are delegated to the driver
 implementation. See [node-mongodb-native mapReduce() documentation](http://mongodb.github.io/node-mongodb-native/api-generated/
collection.html#mapreduce) for more detail about options.
*
* ####Example:
*
*     var o = {};
*     o.map = function () { emit(this.name, 1) }
*     o.reduce = function (k, vals) { return vals.length }
*     User.mapReduce(o, function (err, results) {
*       console.log(results)
*     })
*
* ####Other options:
*
* - 'query' {Object} query filter object.
* - 'sort' {Object} sort input objects using this key
...
```

#### <a name="apidoc.element.mongoose.model.on"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>on (type, listener)](#apidoc.element.mongoose.model.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
 * - 2 = connecting
 * - 3 = disconnecting
 *
 * Each state change emits its associated event name.
 *
 * ####Example
 *
 *     conn.on('connected', callback);
 *     conn.on('disconnected', callback);
 *
 * @property readyState
 * @api public
 */

Object.defineProperty(Connection.prototype, 'readyState', {
...
```

#### <a name="apidoc.element.mongoose.model.once"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>once (type, listener)](#apidoc.element.mongoose.model.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
...
        aggregate(_this._pipeline, options || {});
      decorateCursor(cursor);
      resolve(cursor);
      callback && callback(null, cursor);
    });
    return;
  }
  _this._model.collection.emitter.once('queue', function() {
    var cursor = _this._model.collection.
      aggregate(_this._pipeline, options || {});
    decorateCursor(cursor);
    resolve(cursor);
    callback && callback(null, cursor);
  });
});
...
```

#### <a name="apidoc.element.mongoose.model.populate"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>populate (docs, paths, callback)](#apidoc.element.mongoose.model.populate)
- description and source-code
```javascript
populate = function (docs, paths, callback) {
  var _this = this;
  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  // normalized paths
  var noPromise = paths && !!paths.__noPromise;
  paths = utils.populate(paths);

  // data that should persist across subPopulate calls
  var cache = {};

  if (noPromise) {
    _populate(this, docs, paths, cache, callback);
  } else {
    var Promise = PromiseProvider.get();
    return new Promise.ES6(function(resolve, reject) {
      _populate(_this, docs, paths, cache, function(error, docs) {
        if (error) {
          callback && callback(error);
          reject(error);
        } else {
          callback && callback(null, docs);
          resolve(docs);
        }
      });
    });
  }
}
```
- example usage
```shell
...
* Populates document references, executing the 'callback' when complete.
* If you want to use promises instead, use this function with
* ['execPopulate()'](#document_Document-execPopulate)
*
* ####Example:
*
*     doc
*     .populate('company')
*     .populate({
*       path: 'notes',
*       match: /airline/,
*       select: 'text',
*       model: 'modelName'
*       options: opts
*     }, function (err, user) {
...
```

#### <a name="apidoc.element.mongoose.model.prependListener"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>prependListener (type, listener)](#apidoc.element.mongoose.model.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.prependOnceListener"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>prependOnceListener (type, listener)](#apidoc.element.mongoose.model.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.remove"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>remove (conditions, callback)](#apidoc.element.mongoose.model.remove)
- description and source-code
```javascript
function remove(conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }

  // get the mongodb collection object
  var mq = new this.Query(conditions, {}, this, this.collection);

  if (callback) {
    callback = this.$wrapCallback(callback);
  }

  return mq.remove(callback);
}
```
- example usage
```shell
...
'''

The same goes for removing them:

'''js
BlogPost.findById(myId, function (err, post) {
  if (!err) {
    post.comments[0].remove();
    post.save(function (err) {
      // do something
    });
  }
});
'''
...
```

#### <a name="apidoc.element.mongoose.model.removeAllListeners"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>removeAllListeners (type)](#apidoc.element.mongoose.model.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.removeListener"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>removeListener (type, listener)](#apidoc.element.mongoose.model.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.model.replaceOne"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>replaceOne (conditions, doc, options, callback)](#apidoc.element.mongoose.model.replaceOne)
- description and source-code
```javascript
function replaceOne(conditions, doc, options, callback) {
  return _update(this, 'replaceOne', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.updateOne.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .replaceOne()
 *
 * @param {Function} callback
 * @see Model.replaceOne #model_Model.replaceOne
 * @api private
 */
Query.prototype._replaceOne = function(callback) {
var schema = this.model.schema;
...
```

#### <a name="apidoc.element.mongoose.model.setMaxListeners"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>setMaxListeners (n)](#apidoc.element.mongoose.model.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
...
}

var required = this.schema.requiredPaths();
for (var i = 0; i < required.length; ++i) {
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);

if (!skipInit && obj) {
  this.init(obj);
}

this.$__registerHooksFromSchema();
...
```

#### <a name="apidoc.element.mongoose.model.update"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>update (conditions, doc, options, callback)](#apidoc.element.mongoose.model.update)
- description and source-code
```javascript
function update(conditions, doc, options, callback) {
  return _update(this, 'update', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

/**
* Sends an update command with this document '_id' as the query selector.
*
* ####Example:
*
*     weirdCar.update({$inc: {wheels:1}}, { w: 1 }, callback);
*
* ####Valid options:
*
*  - same as in [Model.update](#model_Model.update)
*
* @see Model.update #model_Model.update
* @param {Object} doc
...
```

#### <a name="apidoc.element.mongoose.model.updateMany"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>updateMany (conditions, doc, options, callback)](#apidoc.element.mongoose.model.updateMany)
- description and source-code
```javascript
function updateMany(conditions, doc, options, callback) {
  return _update(this, 'updateMany', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.update.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .updateMany()
 *
 * @param {Function} callback
 * @see Model.update #model_Model.update
 * @api private
 */
Query.prototype._updateMany = function(callback) {
var schema = this.model.schema;
...
```

#### <a name="apidoc.element.mongoose.model.updateOne"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>updateOne (conditions, doc, options, callback)](#apidoc.element.mongoose.model.updateOne)
- description and source-code
```javascript
function updateOne(conditions, doc, options, callback) {
  return _update(this, 'updateOne', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.updateMany.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .updateOne()
 *
 * @param {Function} callback
 * @see Model.update #model_Model.update
 * @api private
 */
Query.prototype._updateOne = function(callback) {
var schema = this.model.schema;
...
```

#### <a name="apidoc.element.mongoose.model.where"></a>[function <span class="apidocSignatureSpan">mongoose.model.</span>where (path, val)](#apidoc.element.mongoose.model.where)
- description and source-code
```javascript
function where(path, val) {
  void val; // eslint
  // get the mongodb collection object
  var mq = new this.Query({}, {}, this, this.collection).find({});
  return mq.where.apply(mq, arguments);
}
```
- example usage
```shell
...
*
* For example, instead of writing:
*
*     User.find({age: {$gte: 21, $lte: 65}}, callback);
*
* we can instead write:
*
*     User.where('age').gte(21).lte(65).exec(callback);
*
* Since the Query class also supports 'where' you can continue chaining
*
*     User
*     .where('age').gte(21).lte(65)
*     .where('name', /^b/i)
*     ... etc
...
```



# <a name="apidoc.module.mongoose.model.prototype"></a>[module mongoose.model.prototype](#apidoc.module.mongoose.model.prototype)

#### <a name="apidoc.element.mongoose.model.prototype.increment"></a>[function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>increment ()](#apidoc.element.mongoose.model.prototype.increment)
- description and source-code
```javascript
function increment() {
  this.$__.version = VERSION_ALL;
  return this;
}
```
- example usage
```shell
...
// only increment the version if an array position changes.
// modifying elements of an array is ok if position does not change.

if (op === '$push' || op === '$pushAll' || op === '$addToSet') {
  self.$__.version = VERSION_INC;
} else if (/^\$p/.test(op)) {
  // potentially changing array positions
  self.increment();
} else if (Array.isArray(val)) {
  // $set an array
  self.increment();
} else if (/\.\d+\.|\.\d+$/.test(data.path)) {
  // now handling $set, $unset
  // subpath of array
  self.$__.version = VERSION_WHERE;
...
```

#### <a name="apidoc.element.mongoose.model.prototype.model"></a>[function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>model (name)](#apidoc.element.mongoose.model.prototype.model)
- description and source-code
```javascript
function model(name) {
  return this.db.model(name);
}
```
- example usage
```shell
...
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model

Once we define a model through 'mongoose.model('ModelName', mySchema)', we can access it through the same function

'''js
var myModel = mongoose.model('ModelName');
'''

Or just do it all at once
...
```

#### <a name="apidoc.element.mongoose.model.prototype.remove"></a>[function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>remove (options, fn)](#apidoc.element.mongoose.model.prototype.remove)
- description and source-code
```javascript
function remove(options, fn) {
  if (typeof options === 'function') {
    fn = options;
    options = undefined;
  }

  if (!options) {
    options = {};
  }

  if (this.$__.removing) {
    if (fn) {
      this.$__.removing.then(
          function(res) { fn(null, res); },
          function(err) { fn(err); });
    }
    return this;
  }

  var _this = this;
  var Promise = PromiseProvider.get();

  if (fn) {
    fn = this.constructor.$wrapCallback(fn);
  }

  this.$__.removing = new Promise.ES6(function(resolve, reject) {
    var where = _this.$__where();
    if (where instanceof Error) {
      reject(where);
      fn && fn(where);
      return;
    }

    if (!options.safe && _this.schema.options.safe) {
      options.safe = _this.schema.options.safe;
    }

    _this.collection.remove(where, options, function(err) {
      if (!err) {
        _this.emit('remove', _this);
        _this.constructor.emit('remove', _this);
        resolve(_this);
        fn && fn(null, _this);
        return;
      }
      reject(err);
      fn && fn(err);
    });
  });
  return this.$__.removing;
}
```
- example usage
```shell
...
'''

The same goes for removing them:

'''js
BlogPost.findById(myId, function (err, post) {
  if (!err) {
    post.comments[0].remove();
    post.save(function (err) {
      // do something
    });
  }
});
'''
...
```

#### <a name="apidoc.element.mongoose.model.prototype.save"></a>[function <span class="apidocSignatureSpan">mongoose.model.prototype.</span>save (options, fn)](#apidoc.element.mongoose.model.prototype.save)
- description and source-code
```javascript
save = function (options, fn) {
  if (typeof options === 'function') {
    fn = options;
    options = undefined;
  }

  if (!options) {
    options = {};
  }

  if (fn) {
    fn = this.constructor.$wrapCallback(fn);
  }

  return this.$__save(options, fn);
}
```
- example usage
```shell
...
Then Mongoose will create the model for your __tickets__ collection, not your __ticket__ collection.

Once we have our model, we can then instantiate it, and save it:

'''js
var instance = new MyModel();
instance.my.key = 'hello';
instance.save(function (err) {
  //
});
'''

Or we can find documents from the same collection

'''js
...
```



# <a name="apidoc.module.mongoose.promise"></a>[module mongoose.promise](#apidoc.module.mongoose.promise)

#### <a name="apidoc.element.mongoose.promise.promise"></a>[function <span class="apidocSignatureSpan">mongoose.</span>promise (fn)](#apidoc.element.mongoose.promise.promise)
- description and source-code
```javascript
function Promise(fn) {
  MPromise.call(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise.ES6"></a>[function <span class="apidocSignatureSpan">mongoose.promise.</span>ES6 (resolver)](#apidoc.element.mongoose.promise.ES6)
- description and source-code
```javascript
ES6 = function (resolver) {
  var promise = new Promise();

  // No try/catch for backwards compatibility
  resolver(
    function() {
      promise.complete.apply(promise, arguments);
    },
    function(e) {
      promise.error(e);
    });

  return promise;
}
```
- example usage
```shell
...
 * @param {Function} callback
 * @return {Promise}
 */

Aggregate.prototype.explain = function(callback) {
var _this = this;
var Promise = PromiseProvider.get();
return new Promise.ES6(function(resolve, reject) {
  if (!_this._pipeline.length) {
    var err = new Error('Aggregate has empty pipeline');
    if (callback) {
      callback(err);
    }
    reject(err);
    return;
...
```



# <a name="apidoc.module.mongoose.promise.prototype"></a>[module mongoose.promise.prototype](#apidoc.module.mongoose.promise.prototype)

#### <a name="apidoc.element.mongoose.promise.prototype.addBack"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addBack (fn)](#apidoc.element.mongoose.promise.prototype.addBack)
- description and source-code
```javascript
addBack = function (fn) {
  if (!fn) return this;
  if ('function' != typeof fn) throw new TypeError("fn should be a function");
  this.on(Promise.FAILURE, function (err) { fn.call(this, err); });
  this.on(Promise.SUCCESS, function () { fn.apply(this, strongUnshift(null, arguments)); });
  return this;
}
```
- example usage
```shell
...
*     // executing a query explicitly
*     var query = MyModel.find({ name: /john/i }, null, { skip: 10 })
*     query.exec(function (err, docs) {});
*
*     // using the promise returned from executing a query
*     var query = MyModel.find({ name: /john/i }, null, { skip: 10 });
*     var promise = query.exec();
*     promise.addBack(function (err, docs) {});
*
* @param {Object} conditions
* @param {Object} [projection] optional fields to return (http://bit.ly/1HotzBo)
* @param {Object} [options] optional
* @param {Function} [callback]
* @return {Query}
* @see field selection #query_Query-select
...
```

#### <a name="apidoc.element.mongoose.promise.prototype.addCallback"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addCallback (fn)](#apidoc.element.mongoose.promise.prototype.addCallback)
- description and source-code
```javascript
addCallback = function (fn) {
  if (!fn) return this;
  if ('function' != typeof fn) throw new TypeError("fn should be a function");
  return this.on(Promise.SUCCESS, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise.prototype.addErrback"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>addErrback (fn)](#apidoc.element.mongoose.promise.prototype.addErrback)
- description and source-code
```javascript
addErrback = function (fn) {
  if (!fn) return this;
  if ('function' != typeof fn) throw new TypeError("fn should be a function");
  return this.on(Promise.FAILURE, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise.prototype.catch"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>catch (onReject)](#apidoc.element.mongoose.promise.prototype.catch)
- description and source-code
```javascript
catch = function (onReject) {
  return this.then(null, onReject);
}
```
- example usage
```shell
...

Promise.prototype.then = util.deprecate(Promise.prototype.then,
 'Mongoose: mpromise (mongoose\'s default promise library) is deprecated, ' +
 'plug in your own promise library instead: ' +
 'http://mongoosejs.com/docs/promises.html');

/**
* ES6-style '.catch()' shorthand
*
* @method catch
* @memberOf Promise
* @param {Function} onReject
* @return {Promise}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.promise.prototype.complete"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>complete ()](#apidoc.element.mongoose.promise.prototype.complete)
- description and source-code
```javascript
complete = function () {
  return this.safeEmit.apply(this, strongUnshift(Promise.SUCCESS, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise.prototype.error"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>error (err)](#apidoc.element.mongoose.promise.prototype.error)
- description and source-code
```javascript
error = function (err) {
  if (!(err instanceof Error)) {
    if (err instanceof Object) {
      err = util.inspect(err);
    }
    err = new Error(err);
  }
  return this.reject(err);
}
```
- example usage
```shell
...
if (!rgxProtocol.test(host)) {
  host = 'mongodb://' + host;
}

try {
  parsed = muri(host);
} catch (err) {
  this.error(err, callback);
  return new Promise.ES6(function(resolve, reject) {
    reject(err);
  });
}

database = parsed.db;
host = parsed.hosts[0].host || parsed.hosts[0].ipc;
...
```

#### <a name="apidoc.element.mongoose.promise.prototype.resolve"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>resolve (err)](#apidoc.element.mongoose.promise.prototype.resolve)
- description and source-code
```javascript
resolve = function (err) {
  if (err) return this.error(err);
  return this.fulfill.apply(this, Array.prototype.slice.call(arguments, 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise.prototype.then"></a>[function <span class="apidocSignatureSpan">mongoose.promise.prototype.</span>then ()](#apidoc.element.mongoose.promise.prototype.then)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
...
*
* ####Example:
*
*     aggregate.exec(callback);
*
*     // Because a promise is returned, the 'callback' is optional.
*     var promise = aggregate.exec();
*     promise.then(..);
*
* @see Promise #promise_Promise
* @param {Function} [callback]
* @return {Promise}
* @api public
*/
...
```



# <a name="apidoc.module.mongoose.promise_provider"></a>[module mongoose.promise_provider](#apidoc.module.mongoose.promise_provider)

#### <a name="apidoc.element.mongoose.promise_provider._promise"></a>[function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>_promise (fn)](#apidoc.element.mongoose.promise_provider._promise)
- description and source-code
```javascript
function Promise(fn) {
  MPromise.call(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.promise_provider.get"></a>[function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>get ()](#apidoc.element.mongoose.promise_provider.get)
- description and source-code
```javascript
get = function () {
  return Promise._promise;
}
```
- example usage
```shell
...
// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model
...
```

#### <a name="apidoc.element.mongoose.promise_provider.reset"></a>[function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>reset ()](#apidoc.element.mongoose.promise_provider.reset)
- description and source-code
```javascript
reset = function () {
  Promise._promise = MPromise;
}
```
- example usage
```shell
...
 * Set the current promise constructor
 *
 * @api private
 */

Promise.set = function(lib) {
  if (lib === MPromise) {
    return Promise.reset();
  }
  Promise._promise = require('./ES6Promise');
  Promise._promise.use(lib);
  require('mquery').Promise = Promise._promise.ES6;
};

/**
...
```

#### <a name="apidoc.element.mongoose.promise_provider.set"></a>[function <span class="apidocSignatureSpan">mongoose.promise_provider.</span>set (lib)](#apidoc.element.mongoose.promise_provider.set)
- description and source-code
```javascript
set = function (lib) {
  if (lib === MPromise) {
    return Promise.reset();
  }
  Promise._promise = require('./ES6Promise');
  Promise._promise.use(lib);
  require('mquery').Promise = Promise._promise.ES6;
}
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```



# <a name="apidoc.module.mongoose.query"></a>[module mongoose.query](#apidoc.module.mongoose.query)

#### <a name="apidoc.element.mongoose.query.query"></a>[function <span class="apidocSignatureSpan">mongoose.</span>query (conditions, options, model, collection)](#apidoc.element.mongoose.query.query)
- description and source-code
```javascript
function Query(conditions, options, model, collection) {
  // this stuff is for dealing with custom queries created by #toConstructor
  if (!this._mongooseOptions) {
    this._mongooseOptions = {};
  }

  // this is the case where we have a CustomQuery, we need to check if we got
  // options passed in, and if we did, merge them in
  if (options) {
    var keys = Object.keys(options);
    for (var i = 0; i < keys.length; ++i) {
      var k = keys[i];
      this._mongooseOptions[k] = options[k];
    }
  }

  if (collection) {
    this.mongooseCollection = collection;
  }

  if (model) {
    this.model = model;
    this.schema = model.schema;
  }

  // this is needed because map reduce returns a model that can be queried, but
  // all of the queries on said model should be lean
  if (this.model && this.model._mapreduce) {
    this.lean();
  }

  // inherit mquery
  mquery.call(this, this.mongooseCollection, options);

  if (conditions) {
    this.find(conditions);
  }

  if (this.schema) {
    var kareemOptions = {
      useErrorHandlers: true,
      numCallbackParams: 1
    };
    this._count = this.model.hooks.createWrapper('count',
        Query.prototype._count, this, kareemOptions);
    this._execUpdate = this.model.hooks.createWrapper('update',
        Query.prototype._execUpdate, this, kareemOptions);
    this._find = this.model.hooks.createWrapper('find',
        Query.prototype._find, this, kareemOptions);
    this._findOne = this.model.hooks.createWrapper('findOne',
        Query.prototype._findOne, this, kareemOptions);
    this._findOneAndRemove = this.model.hooks.createWrapper('findOneAndRemove',
        Query.prototype._findOneAndRemove, this, kareemOptions);
    this._findOneAndUpdate = this.model.hooks.createWrapper('findOneAndUpdate',
        Query.prototype._findOneAndUpdate, this, kareemOptions);
    this._replaceOne = this.model.hooks.createWrapper('replaceOne',
        Query.prototype._replaceOne, this, kareemOptions);
    this._updateMany = this.model.hooks.createWrapper('updateMany',
        Query.prototype._updateMany, this, kareemOptions);
    this._updateOne = this.model.hooks.createWrapper('updateOne',
        Query.prototype._updateOne, this, kareemOptions);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.query.prototype"></a>[module mongoose.query.prototype](#apidoc.module.mongoose.query.prototype)

#### <a name="apidoc.element.mongoose.query.prototype._applyPaths"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_applyPaths ()](#apidoc.element.mongoose.query.prototype._applyPaths)
- description and source-code
```javascript
function applyPaths() {
  this._fields = this._fields || {};
  helpers.applyPaths(this._fields, this.model.schema);
}
```
- example usage
```shell
...
 */
Query.prototype._find = function(callback) {
if (this._castError) {
  callback(this._castError);
  return this;
}

this._applyPaths();
this._fields = this._castFields(this._fields);

var fields = this._fieldsForExec();
var options = this._mongooseOptions;
var _this = this;

var cb = function(err, docs) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype._castFields"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_castFields (fields)](#apidoc.element.mongoose.query.prototype._castFields)
- description and source-code
```javascript
function _castFields(fields) {
  var selected,
      elemMatchKeys,
      keys,
      key,
      out,
      i;

  if (fields) {
    keys = Object.keys(fields);
    elemMatchKeys = [];
    i = keys.length;

    // collect $elemMatch args
    while (i--) {
      key = keys[i];
      if (fields[key].$elemMatch) {
        selected || (selected = {});
        selected[key] = fields[key];
        elemMatchKeys.push(key);
      }
    }
  }

  if (selected) {
    // they passed $elemMatch, cast em
    try {
      out = this.cast(this.model, selected);
    } catch (err) {
      return err;
    }

    // apply the casted field args
    i = elemMatchKeys.length;
    while (i--) {
      key = elemMatchKeys[i];
      fields[key] = out[key];
    }
  }

  return fields;
}
```
- example usage
```shell
...
Query.prototype._find = function(callback) {
if (this._castError) {
  callback(this._castError);
  return this;
}

this._applyPaths();
this._fields = this._castFields(this._fields);

var fields = this._fieldsForExec();
var options = this._mongooseOptions;
var _this = this;

var cb = function(err, docs) {
  if (err) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype._castUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_castUpdate (obj, overwrite)](#apidoc.element.mongoose.query.prototype._castUpdate)
- description and source-code
```javascript
function _castUpdate(obj, overwrite) {
  var strict;
  if ('strict' in this._mongooseOptions) {
    strict = this._mongooseOptions.strict;
  } else if (this.schema && this.schema.options) {
    strict = this.schema.options.strict;
  } else {
    strict = true;
  }
  return castUpdate(this.schema, obj, {
    overwrite: overwrite,
    strict: strict
  });
}
```
- example usage
```shell
...
// validate the update part of the query
var castedDoc;
try {
  var $options = {retainKeyOrder: true};
  if (options && options.minimize) {
    $options.minimize = true;
  }
  castedDoc = query._castUpdate(utils.clone(doc, $options),
    (options && options.overwrite) || op === 'replaceOne');
} catch (err) {
  query._castError = castedQuery;
  if (callback) {
    callback(err);
    return query;
  } else if (!options || !options.dontThrowCastError) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype._count"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_count (callback)](#apidoc.element.mongoose.query.prototype._count)
- description and source-code
```javascript
_count = function (callback) {
  try {
    this.cast(this.model);
  } catch (err) {
    process.nextTick(function() {
      callback(err);
    });
    return this;
  }

  var conds = this._conditions;
  var options = this._optionsForExec();

  this._collection.count(conds, options, utils.tick(callback));
}
```
- example usage
```shell
...
 }

 this.op = 'count';
 if (!callback) {
   return this;
 }

 this._count(callback);

 return this;
};

/**
* Declares or executes a distict() operation.
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype._execUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_execUpdate (callback)](#apidoc.element.mongoose.query.prototype._execUpdate)
- description and source-code
```javascript
_execUpdate = function (callback) {
  var schema = this.model.schema;
  var doValidate;
  var _this;

  var castedQuery = this._conditions;
  var castedDoc = this._update;
  var options = this.options;

  if (this._castError) {
    callback(this._castError);
    return this;
  }

  if (this.options.runValidators) {
    _this = this;
    doValidate = updateValidators(this, schema, castedDoc, options);
    var _callback = function(err) {
      if (err) {
        return callback(err);
      }

      Query.base.update.call(_this, castedQuery, castedDoc, options, callback);
    };
    try {
      doValidate(_callback);
    } catch (err) {
      process.nextTick(function() {
        callback(err);
      });
    }
    return this;
  }

  Query.base.update.call(this, castedQuery, castedDoc, options, callback);
  return this;
}
```
- example usage
```shell
...
  if (!query._update) {
    query._update = castedDoc;
  }

  // Hooks
  if (callback) {
    if (op === 'update') {
      return query._execUpdate(callback);
    }
    return query['_' + op](callback);
  }

  return Query.base[op].call(query, castedQuery, castedDoc, options, callback);
}
...
```

#### <a name="apidoc.element.mongoose.query.prototype._find"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_find (callback)](#apidoc.element.mongoose.query.prototype._find)
- description and source-code
```javascript
_find = function (callback) {
  if (this._castError) {
    callback(this._castError);
    return this;
  }

  this._applyPaths();
  this._fields = this._castFields(this._fields);

  var fields = this._fieldsForExec();
  var options = this._mongooseOptions;
  var _this = this;

  var cb = function(err, docs) {
    if (err) {
      return callback(err);
    }

    if (docs.length === 0) {
      return callback(null, docs);
    }

    if (!options.populate) {
      return options.lean === true
          ? callback(null, docs)
          : completeMany(_this.model, docs, fields, null, callback);
    }

    var pop = helpers.preparePopulationOptionsMQ(_this, options);
    pop.__noPromise = true;
    _this.model.populate(docs, pop, function(err, docs) {
      if (err) return callback(err);
      return options.lean === true
          ? callback(null, docs)
          : completeMany(_this.model, docs, fields, pop, callback);
    });
  };

  return Query.base.find.call(this, {}, cb);
}
```
- example usage
```shell
...
 }

 // if we don't have a callback, then just return the query object
 if (!callback) {
   return Query.base.find.call(this);
 }

 this._find(callback);

 return this;
};

/**
* Merges another Query or conditions object into this one.
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype._findAndModify"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findAndModify (type, callback)](#apidoc.element.mongoose.query.prototype._findAndModify)
- description and source-code
```javascript
_findAndModify = function (type, callback) {
  if (typeof callback !== 'function') {
    throw new Error('Expected callback in _findAndModify');
  }

  var model = this.model;
  var schema = model.schema;
  var _this = this;
  var castedQuery;
  var castedDoc;
  var fields;
  var opts;
  var doValidate;

  castedQuery = castQuery(this);
  if (castedQuery instanceof Error) {
    return callback(castedQuery);
  }

  opts = this._optionsForExec(model);

  if ('strict' in opts) {
    this._mongooseOptions.strict = opts.strict;
  }

  if (type === 'remove') {
    opts.remove = true;
  } else {
    if (!('new' in opts)) {
      opts.new = false;
    }
    if (!('upsert' in opts)) {
      opts.upsert = false;
    }
    if (opts.upsert || opts['new']) {
      opts.remove = false;
    }

    castedDoc = castDoc(this, opts.overwrite);
    castedDoc = setDefaultsOnInsert(this, schema, castedDoc, opts);
    if (!castedDoc) {
      if (opts.upsert) {
        // still need to do the upsert to empty doc
        var doc = utils.clone(castedQuery);
        delete doc._id;
        castedDoc = {$set: doc};
      } else {
        return this.findOne(callback);
      }
    } else if (castedDoc instanceof Error) {
      return callback(castedDoc);
    } else {
      // In order to make MongoDB 2.6 happy (see
      // https://jira.mongodb.org/browse/SERVER-12266 and related issues)
      // if we have an actual update document but $set is empty, junk the $set.
      if (castedDoc.$set && Object.keys(castedDoc.$set).length === 0) {
        delete castedDoc.$set;
      }
    }

    doValidate = updateValidators(this, schema, castedDoc, opts);
  }

  this._applyPaths();

  var options = this._mongooseOptions;

  if (this._fields) {
    fields = utils.clone(this._fields);
    opts.fields = this._castFields(fields);
    if (opts.fields instanceof Error) {
      return callback(opts.fields);
    }
  }

  if (opts.sort) convertSortToArray(opts);

  var cb = function(err, doc, res) {
    if (err) {
      return callback(err);
    }

    if (!doc || (utils.isObject(doc) && Object.keys(doc).length === 0)) {
      if (opts.rawResult) {
        return callback(null, res);
      }
      // opts.passRawResult will be deprecated soon
      if (opts.passRawResult) {
        return callback(null, null, decorateResult(res));
      }
      return callback(null, null);
    }

    if (!options.populate) {
      if (options.lean === true) {
        return _completeOneLean(doc, res, opts, callback);
      }
      return completeOne(_this.model, doc, res, opts, fields, null, callback);
    }

    var pop = helpers.preparePopulationOptionsMQ(_this, options);
    pop.__noPromise = true;
    _this.model.populate(doc, pop, function(err, doc) {
      if (err) {
        return callback(err);
      }

      if (options.lean === true) {
        return _completeOneLean(doc, res, opts, callback);
      }
      return completeOne(_this.model, doc, res, opts, fields, pop, callback);
    });
  };

  if (opts.runValidators && doValidate) {
    var _callback = function(error) {
      if (error) {
        return callback(error);
      }
      _this._collection.findAndModify(castedQuery, castedDoc, opts, utils.tick(function(error, res) {
        return cb(error, res ? res.value : res, res);
      }));
    };

    try {
      doValidate(_callback);
    } catch (error) {
      callback(error);
    }
  } else {
    this._collection.findAndModify(castedQuery, castedDoc, opts, utils.tick(function(error, res) {
      return cb(error, res ? res.value : res, res);
    }));
  }

  return this;
}
```
- example usage
```shell
...
* Thunk around findOneAndUpdate()
*
* @param {Function} [callback]
* @api private
*/

Query.prototype._findOneAndUpdate = function(callback) {
 this._findAndModify('update', callback);
 return this;
};

/**
* Issues a mongodb [findAndModify](http://www.mongodb.org/display/DOCS/findAndModify+Command) remove command.
*
* Finds a matching document, removes it, passing the found document (if any) to the callback. Executes immediately if 'callback'
is passed.
...
```

#### <a name="apidoc.element.mongoose.query.prototype._findOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOne (callback)](#apidoc.element.mongoose.query.prototype._findOne)
- description and source-code
```javascript
_findOne = function (callback) {
  if (this._castError) {
    return callback(this._castError);
  }

  this._applyPaths();
  this._fields = this._castFields(this._fields);

  var options = this._mongooseOptions;
  var projection = this._fieldsForExec();
  var _this = this;

  // don't pass in the conditions because we already merged them in
  Query.base.findOne.call(_this, {}, function(err, doc) {
    if (err) {
      return callback(err);
    }
    if (!doc) {
      return callback(null, null);
    }

    if (!options.populate) {
      return options.lean === true
          ? callback(null, doc)
          : completeOne(_this.model, doc, null, {}, projection, null, callback);
    }

    var pop = helpers.preparePopulationOptionsMQ(_this, options);
    pop.__noPromise = true;
    _this.model.populate(doc, pop, function(err, doc) {
      if (err) {
        return callback(err);
      }
      return options.lean === true
          ? callback(null, doc)
          : completeOne(_this.model, doc, null, {}, projection, pop, callback);
    });
  });
}
```
- example usage
```shell
...
 }

 if (!callback) {
   // already merged in the conditions, don't need to send them in.
   return Query.base.findOne.call(this);
 }

 this._findOne(callback);

 return this;
};

/**
* Thunk around count()
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype._findOneAndRemove"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOneAndRemove (callback)](#apidoc.element.mongoose.query.prototype._findOneAndRemove)
- description and source-code
```javascript
_findOneAndRemove = function (callback) {
  Query.base.findOneAndRemove.call(this, callback);
}
```
- example usage
```shell
...

 options && this.setOptions(options);

 if (!callback) {
   return this;
 }

 this._findOneAndRemove(callback);

 return this;
};

/*!
* Thunk around findOneAndRemove()
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype._findOneAndUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_findOneAndUpdate (callback)](#apidoc.element.mongoose.query.prototype._findOneAndUpdate)
- description and source-code
```javascript
_findOneAndUpdate = function (callback) {
  this._findAndModify('update', callback);
  return this;
}
```
- example usage
```shell
...
   this.setOptions(options);
 }

 if (!callback) {
   return this;
 }

 return this._findOneAndUpdate(callback);
};

/*!
* Thunk around findOneAndUpdate()
*
* @param {Function} [callback]
* @api private
...
```

#### <a name="apidoc.element.mongoose.query.prototype._mergeUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_mergeUpdate (doc)](#apidoc.element.mongoose.query.prototype._mergeUpdate)
- description and source-code
```javascript
_mergeUpdate = function (doc) {
  if (!this._update) this._update = {};
  if (doc instanceof Query) {
    if (doc._update) {
      utils.mergeClone(this._update, doc._update);
    }
  } else {
    utils.mergeClone(this._update, doc);
  }
}
```
- example usage
```shell
...

if (mquery.canMerge(criteria)) {
  this.merge(criteria);
}

// apply doc
if (doc) {
  this._mergeUpdate(doc);
}

if (options) {
  options = utils.clone(options, { retainKeyOrder: true });
  if (options.projection) {
    this.select(options.projection);
    delete options.projection;
...
```

#### <a name="apidoc.element.mongoose.query.prototype._optionsForExec"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_optionsForExec (model)](#apidoc.element.mongoose.query.prototype._optionsForExec)
- description and source-code
```javascript
_optionsForExec = function (model) {
  var options = Query.base._optionsForExec.call(this);

  delete options.populate;
  delete options.retainKeyOrder;
  model = model || this.model;

  if (!model) {
    return options;
  }

  if (!('safe' in options) && model.schema.options.safe) {
    options.safe = model.schema.options.safe;
  }

  if (!('readPreference' in options) && model.schema.options.read) {
    options.readPreference = model.schema.options.read;
  }

  return options;
}
```
- example usage
```shell
...
   process.nextTick(function() {
     callback(err);
   });
   return this;
 }

 var conds = this._conditions;
 var options = this._optionsForExec();

 this._collection.count(conds, options, utils.tick(callback));
};

/**
* Specifying this query as a 'count' query.
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype._replaceOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_replaceOne (callback)](#apidoc.element.mongoose.query.prototype._replaceOne)
- description and source-code
```javascript
_replaceOne = function (callback) {
  var schema = this.model.schema;
  var doValidate;
  var _this;

  var castedQuery = this._conditions;
  var castedDoc = this._update;
  var options = this.options;

  if (this._castError) {
    callback(this._castError);
    return this;
  }

  if (this.options.runValidators) {
    _this = this;
    doValidate = updateValidators(this, schema, castedDoc, options);
    var _callback = function(err) {
      if (err) {
        return callback(err);
      }

      Query.base.updateMany.call(_this, castedQuery, castedDoc, options, callback);
    };
    try {
      doValidate(_callback);
    } catch (err) {
      process.nextTick(function() {
        callback(err);
      });
    }
    return this;
  }

  Query.base.replaceOne.call(this, castedQuery, castedDoc, options, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype._updateForExec"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateForExec ()](#apidoc.element.mongoose.query.prototype._updateForExec)
- description and source-code
```javascript
_updateForExec = function () {
  var update = utils.clone(this._update, {
    retainKeyOrder: true,
    transform: false,
    depopulate: true
  });
  var ops = Object.keys(update);
  var i = ops.length;
  var ret = {};

  while (i--) {
    var op = ops[i];

    if (this.options.overwrite) {
      ret[op] = update[op];
      continue;
    }

    if ('$' !== op[0]) {
      // fix up $set sugar
      if (!ret.$set) {
        if (update.$set) {
          ret.$set = update.$set;
        } else {
          ret.$set = {};
        }
      }
      ret.$set[op] = update[op];
      ops.splice(i, 1);
      if (!~ops.indexOf('$set')) ops.push('$set');
    } else if ('$set' === op) {
      if (!ret.$set) {
        ret[op] = update[op];
      }
    } else {
      ret[op] = update[op];
    }
  }

  return ret;
}
```
- example usage
```shell
...

// if doc is undefined at this point, this means this function is being
// executed by exec(not always see below). Grab the update doc from here in
// order to validate
// This could also be somebody calling update() or update({}). Probably not a
// common use case, check for _update to make sure we don't do anything bad
if (!doc && query._update) {
  doc = query._updateForExec();
}

if (mquery.canMerge(conditions)) {
  query.merge(conditions);
}

// validate the selector part of the query
...
```

#### <a name="apidoc.element.mongoose.query.prototype._updateMany"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateMany (callback)](#apidoc.element.mongoose.query.prototype._updateMany)
- description and source-code
```javascript
_updateMany = function (callback) {
  var schema = this.model.schema;
  var doValidate;
  var _this;

  var castedQuery = this._conditions;
  var castedDoc = this._update;
  var options = this.options;

  if (this._castError) {
    callback(this._castError);
    return this;
  }

  if (this.options.runValidators) {
    _this = this;
    doValidate = updateValidators(this, schema, castedDoc, options);
    var _callback = function(err) {
      if (err) {
        return callback(err);
      }

      Query.base.updateMany.call(_this, castedQuery, castedDoc, options, callback);
    };
    try {
      doValidate(_callback);
    } catch (err) {
      process.nextTick(function() {
        callback(err);
      });
    }
    return this;
  }

  Query.base.updateMany.call(this, castedQuery, castedDoc, options, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype._updateOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>_updateOne (callback)](#apidoc.element.mongoose.query.prototype._updateOne)
- description and source-code
```javascript
_updateOne = function (callback) {
  var schema = this.model.schema;
  var doValidate;
  var _this;

  var castedQuery = this._conditions;
  var castedDoc = this._update;
  var options = this.options;

  if (this._castError) {
    callback(this._castError);
    return this;
  }

  if (this.options.runValidators) {
    _this = this;
    doValidate = updateValidators(this, schema, castedDoc, options);
    var _callback = function(err) {
      if (err) {
        return callback(err);
      }

      Query.base.updateOne.call(_this, castedQuery, castedDoc, options, callback);
    };
    try {
      doValidate(_callback);
    } catch (err) {
      process.nextTick(function() {
        callback(err);
      });
    }
    return this;
  }

  Query.base.updateOne.call(this, castedQuery, castedDoc, options, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype.box"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>box (ll, ur)](#apidoc.element.mongoose.query.prototype.box)
- description and source-code
```javascript
box = function (ll, ur) {
  if (!Array.isArray(ll) && utils.isObject(ll)) {
    ur = ll.ur;
    ll = ll.ll;
  }
  return Query.base.box.call(this, ll, ur);
}
```
- example usage
```shell
...
*/

/**
* Defines a '$within' or '$geoWithin' argument for geo-spatial queries.
*
* ####Example
*
*     query.where(path).within().box()
*     query.where(path).within().circle()
*     query.where(path).within().geometry()
*
*     query.where('loc').within({ center: [50,50], radius: 10, unique: true, spherical: true });
*     query.where('loc').within({ box: [[40.73, -73.9], [40.7, -73.988]] });
*     query.where('loc').within({ polygon: [[],[],[],[]] });
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype.cast"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>cast (model, obj)](#apidoc.element.mongoose.query.prototype.cast)
- description and source-code
```javascript
cast = function (model, obj) {
  obj || (obj = this._conditions);

  try {
    return cast(model.schema, obj, {
      upsert: this.options && this.options.upsert,
      strict: (this.options && this.options.strict) ||
        (model.schema.options && model.schema.options.strict)
    });
  } catch (err) {
    // CastError, assign model
    if (typeof err.setModel === 'function') {
      err.setModel(model);
    }
    throw err;
  }
}
```
- example usage
```shell
...
  init(self, obj[i], doc[i], path + '.');
} else {
  if (obj[i] === null) {
    doc[i] = null;
  } else if (obj[i] !== undefined) {
    if (schema) {
      try {
        doc[i] = schema.cast(obj[i], self, true);
      } catch (e) {
        self.invalidate(e.path, new ValidatorError({
          path: e.path,
          message: e.message,
          type: 'cast',
          value: e.value
        }));
...
```

#### <a name="apidoc.element.mongoose.query.prototype.catch"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>catch (reject)](#apidoc.element.mongoose.query.prototype.catch)
- description and source-code
```javascript
catch = function (reject) {
  return this.exec().then(null, reject);
}
```
- example usage
```shell
...

Promise.prototype.then = util.deprecate(Promise.prototype.then,
 'Mongoose: mpromise (mongoose\'s default promise library) is deprecated, ' +
 'plug in your own promise library instead: ' +
 'http://mongoosejs.com/docs/promises.html');

/**
* ES6-style '.catch()' shorthand
*
* @method catch
* @memberOf Promise
* @param {Function} onReject
* @return {Promise}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.center"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>center ()](#apidoc.element.mongoose.query.prototype.center)
- description and source-code
```javascript
center = function () {
  var path, val;

  if (1 === arguments.length) {
    this._ensurePath('circle');
    path = this._path;
    val = arguments[0];
  } else if (2 === arguments.length) {
    path = arguments[0];
    val = arguments[1];
  } else {
    throw new TypeError("Invalid argument");
  }

  if (!('radius' in val && val.center))
    throw new Error('center and radius are required');

  var conds = this._conditions[path] || (this._conditions[path] = {});

  var type = val.spherical
    ? '$centerSphere'
    : '$center';

  var wKey = this._geoComparison || $withinCmd;
  conds[wKey] = {};
  conds[wKey][type] = [val.center, val.radius];

  if ('unique' in val)
    conds[wKey].$uniqueDocs = !! val.unique;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype.centerSphere"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>centerSphere ()](#apidoc.element.mongoose.query.prototype.centerSphere)
- description and source-code
```javascript
centerSphere = function () {
  if (arguments[0] && arguments[0].constructor.name === 'Object') {
    arguments[0].spherical = true;
  }

  if (arguments[1] && arguments[1].constructor.name === 'Object') {
    arguments[1].spherical = true;
  }

  Query.base.circle.apply(this, arguments);
}
```
- example usage
```shell
...
* _DEPRECATED_ Specifies a $centerSphere condition
*
* **Deprecated.** Use [circle](#query_Query-circle) instead.
*
* ####Example
*
*     var area = { center: [50, 50], radius: 10 };
*     query.where('loc').within().centerSphere(area);
*
* @deprecated
* @param {String} [path]
* @param {Object} val
* @return {Query} this
* @see http://www.mongodb.org/display/DOCS/Geospatial+Indexing
* @see $centerSphere http://docs.mongodb.org/manual/reference/operator/centerSphere/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.collation"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>collation (value)](#apidoc.element.mongoose.query.prototype.collation)
- description and source-code
```javascript
collation = function (value) {
  if (this.options == null) {
    this.options = {};
  }
  this.options.collation = value;
  return this;
}
```
- example usage
```shell
...
};

/**
 * Adds a collation
 *
 * ####Example:
 *
 *     Model.aggregate(..).collation({ locale: 'en_US', strength: 1 }).exec();
 *
 * @param {Object} collation options
 * @param {Boolean} value
 * @see mongodb http://mongodb.github.io/node-mongodb-native/2.2/api/Collection.html#aggregate
 */

Aggregate.prototype.collation = function(collation) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>constructor (conditions, options, model, collection)](#apidoc.element.mongoose.query.prototype.constructor)
- description and source-code
```javascript
function Query(conditions, options, model, collection) {
  // this stuff is for dealing with custom queries created by #toConstructor
  if (!this._mongooseOptions) {
    this._mongooseOptions = {};
  }

  // this is the case where we have a CustomQuery, we need to check if we got
  // options passed in, and if we did, merge them in
  if (options) {
    var keys = Object.keys(options);
    for (var i = 0; i < keys.length; ++i) {
      var k = keys[i];
      this._mongooseOptions[k] = options[k];
    }
  }

  if (collection) {
    this.mongooseCollection = collection;
  }

  if (model) {
    this.model = model;
    this.schema = model.schema;
  }

  // this is needed because map reduce returns a model that can be queried, but
  // all of the queries on said model should be lean
  if (this.model && this.model._mapreduce) {
    this.lean();
  }

  // inherit mquery
  mquery.call(this, this.mongooseCollection, options);

  if (conditions) {
    this.find(conditions);
  }

  if (this.schema) {
    var kareemOptions = {
      useErrorHandlers: true,
      numCallbackParams: 1
    };
    this._count = this.model.hooks.createWrapper('count',
        Query.prototype._count, this, kareemOptions);
    this._execUpdate = this.model.hooks.createWrapper('update',
        Query.prototype._execUpdate, this, kareemOptions);
    this._find = this.model.hooks.createWrapper('find',
        Query.prototype._find, this, kareemOptions);
    this._findOne = this.model.hooks.createWrapper('findOne',
        Query.prototype._findOne, this, kareemOptions);
    this._findOneAndRemove = this.model.hooks.createWrapper('findOneAndRemove',
        Query.prototype._findOneAndRemove, this, kareemOptions);
    this._findOneAndUpdate = this.model.hooks.createWrapper('findOneAndUpdate',
        Query.prototype._findOneAndUpdate, this, kareemOptions);
    this._replaceOne = this.model.hooks.createWrapper('replaceOne',
        Query.prototype._replaceOne, this, kareemOptions);
    this._updateMany = this.model.hooks.createWrapper('updateMany',
        Query.prototype._updateMany, this, kareemOptions);
    this._updateOne = this.model.hooks.createWrapper('updateOne',
        Query.prototype._updateOne, this, kareemOptions);
  }
}
```
- example usage
```shell
...
}

if (obj.constructor) {
  switch (exports.getFunctionName(obj.constructor)) {
    case 'Object':
      return cloneObject(obj, options);
    case 'Date':
      return new obj.constructor(+obj);
    case 'RegExp':
      return cloneRegExp(obj);
    default:
      // ignore
      break;
  }
}
...
```

#### <a name="apidoc.element.mongoose.query.prototype.count"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>count (conditions, callback)](#apidoc.element.mongoose.query.prototype.count)
- description and source-code
```javascript
count = function (conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = undefined;
  }

  if (mquery.canMerge(conditions)) {
    this.merge(conditions);
  }

  this.op = 'count';
  if (!callback) {
    return this;
  }

  this._count(callback);

  return this;
}
```
- example usage
```shell
...
};

/**
* Counts number of matching documents in a database collection.
*
* ####Example:
*
*     Adventure.count({ type: 'jungle' }, function (err, count) {
*       if (err) ..
*       console.log('there are %d jungle adventures', count);
*     });
*
* @param {Object} conditions
* @param {Function} [callback]
* @return {Query}
...
```

#### <a name="apidoc.element.mongoose.query.prototype.cursor"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>cursor (opts)](#apidoc.element.mongoose.query.prototype.cursor)
- description and source-code
```javascript
function cursor(opts) {
  this._applyPaths();
  this._fields = this._castFields(this._fields);
  this.setOptions({ fields: this._fieldsForExec() });
  if (opts) {
    this.setOptions(opts);
  }

  try {
    this.cast(this.model);
  } catch (err) {
    return (new QueryCursor(this, this.options))._markError(err);
  }

  return new QueryCursor(this, this.options);
}
```
- example usage
```shell
...
/**
* Sets the cursor option option for the aggregation query (ignored for < 2.6.0).
* Note the different syntax below: .exec() returns a cursor object, and no callback
* is necessary.
*
* ####Example:
*
*     var cursor = Model.aggregate(..).cursor({ batchSize: 1000 }).exec();
*     cursor.each(function(error, doc) {
*       // use doc
*     });
*
* @param {Object} options set the cursor batch size
* @see mongodb http://mongodb.github.io/node-mongodb-native/2.0/api/AggregationCursor.html
*/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.deleteMany"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>deleteMany (cond, callback)](#apidoc.element.mongoose.query.prototype.deleteMany)
- description and source-code
```javascript
deleteMany = function (cond, callback) {
  if (typeof cond === 'function') {
    callback = cond;
    cond = null;
  }

  var cb = typeof callback === 'function';

  try {
    this.cast(this.model);
  } catch (err) {
    if (cb) return process.nextTick(callback.bind(null, err));
    return this;
  }

  return Query.base.deleteMany.call(this, cond, callback);
}
```
- example usage
```shell
...
/**
* Deletes the first document that matches 'conditions' from the collection.
* Behaves like 'remove()', but deletes all documents that match 'conditions'
* regardless of the 'justOne' option.
*
* ####Example:
*
*     Character.deleteMany({ name: /Stark/, age: { $gte: 18 } }, function (err) {});
*
* ####Note:
*
* Like 'Model.remove()', this function does **not** trigger 'pre('remove')' or 'post('remove')' hooks.
*
* @param {Object} conditions
* @param {Function} [callback]
...
```

#### <a name="apidoc.element.mongoose.query.prototype.deleteOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>deleteOne (cond, callback)](#apidoc.element.mongoose.query.prototype.deleteOne)
- description and source-code
```javascript
deleteOne = function (cond, callback) {
  if (typeof cond === 'function') {
    callback = cond;
    cond = null;
  }

  var cb = typeof callback === 'function';

  try {
    this.cast(this.model);
  } catch (err) {
    if (cb) return process.nextTick(callback.bind(null, err));
    return this;
  }

  return Query.base.deleteOne.call(this, cond, callback);
}
```
- example usage
```shell
...
/**
* Deletes the first document that matches 'conditions' from the collection.
* Behaves like 'remove()', but deletes at most one document regardless of the
* 'justOne' option.
*
* ####Example:
*
*     Character.deleteOne({ name: 'Eddard Stark' }, function (err) {});
*
* ####Note:
*
* Like 'Model.remove()', this function does **not** trigger 'pre('remove')' or 'post('remove')' hooks.
*
* @param {Object} conditions
* @param {Function} [callback]
...
```

#### <a name="apidoc.element.mongoose.query.prototype.distinct"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>distinct (field, conditions, callback)](#apidoc.element.mongoose.query.prototype.distinct)
- description and source-code
```javascript
distinct = function (field, conditions, callback) {
  if (!callback) {
    if (typeof conditions === 'function') {
      callback = conditions;
      conditions = undefined;
    } else if (typeof field === 'function') {
      callback = field;
      field = undefined;
      conditions = undefined;
    }
  }

  conditions = utils.toObject(conditions);

  if (mquery.canMerge(conditions)) {
    this.merge(conditions);
  }

  try {
    this.cast(this.model);
  } catch (err) {
    if (!callback) {
      throw err;
    }
    callback(err);
    return this;
  }

  return Query.base.distinct.call(this, {}, field, callback);
}
```
- example usage
```shell
...
/**
* Creates a Query for a 'distinct' operation.
*
* Passing a 'callback' immediately executes the query.
*
* ####Example
*
*     Link.distinct('url', { clicks: {$gt: 100}}, function (err, result) {
*       if (err) return handleError(err);
*
*       assert(Array.isArray(result));
*       console.log('unique urls with more than 100 clicks', result);
*     })
*
*     var query = Link.distinct('url');
...
```

#### <a name="apidoc.element.mongoose.query.prototype.exec"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>exec (op, callback)](#apidoc.element.mongoose.query.prototype.exec)
- description and source-code
```javascript
function exec(op, callback) {
  var Promise = PromiseProvider.get();
  var _this = this;

  if (typeof op === 'function') {
    callback = op;
    op = null;
  } else if (typeof op === 'string') {
    this.op = op;
  }

  var _results;
  var promise = new Promise.ES6(function(resolve, reject) {
    if (!_this.op) {
      resolve();
      return;
    }

    _this[_this.op].call(_this, function(error, res) {
      if (error) {
        reject(error);
        return;
      }
      _results = arguments;
      resolve(res);
    });
  });

  if (callback) {
    promise.then(
      function() {
        callback.apply(null, _results);
        return null;
      },
      function(error) {
        callback(error);
      }).
      catch(function(error) {
        // If we made it here, we must have an error in the callback re:
        // gh-4500, so we need to emit.
        setImmediate(function() {
          _this.model.emit('error', error);
        });
      });
  }

  return promise;
}
```
- example usage
```shell
...

/**
* ES6 Promise wrapper constructor.
*
* Promises are returned from executed queries. Example:
*
*     var query = Candy.find({ bar: true });
*     var promise = query.exec();
*
* DEPRECATED. Mongoose 5.0 will use native promises by default (or bluebird,
* if native promises are not present) but still
* support plugging in your own ES6-compatible promises library. Mongoose 5.0
* will **not** support mpromise.
*
* @param {Function} fn a function which will be called when the promise is resolved that accepts 'fn(err, ...){}' as signature
...
```

#### <a name="apidoc.element.mongoose.query.prototype.find"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>find (conditions, callback)](#apidoc.element.mongoose.query.prototype.find)
- description and source-code
```javascript
find = function (conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }

  conditions = utils.toObject(conditions);

  if (mquery.canMerge(conditions)) {
    this.merge(conditions);
  }

  prepareDiscriminatorCriteria(this);

  try {
    this.cast(this.model);
    this._castError = null;
  } catch (err) {
    this._castError = err;
  }

  // if we don't have a callback, then just return the query object
  if (!callback) {
    return Query.base.find.call(this);
  }

  this._find(callback);

  return this;
}
```
- example usage
```shell
...
  //
});
'''

Or we can find documents from the same collection

'''js
MyModel.find({}, function (err, docs) {
  // docs.forEach
});
'''

You can also 'findOne', 'findById', 'update', etc. For more details check out [the docs](http://mongoosejs.com/docs/queries.html
).

**Important!** If you opened a separate connection using 'mongoose.createConnection()' but attempt to access the model through '
mongoose.model('ModelName')' it will not work as expected since it is not hooked up to an active db connection. In this case access
 your model through the connection you created:
...
```

#### <a name="apidoc.element.mongoose.query.prototype.findOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOne (conditions, projection, options, callback)](#apidoc.element.mongoose.query.prototype.findOne)
- description and source-code
```javascript
findOne = function (conditions, projection, options, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = null;
    projection = null;
    options = null;
  } else if (typeof projection === 'function') {
    callback = projection;
    options = null;
    projection = null;
  } else if (typeof options === 'function') {
    callback = options;
    options = null;
  }

  // make sure we don't send in the whole Document to merge()
  conditions = utils.toObject(conditions);

  this.op = 'findOne';

  if (options) {
    this.setOptions(options);
  }

  if (projection) {
    this.select(projection);
  }

  if (mquery.canMerge(conditions)) {
    this.merge(conditions);
  } else if (conditions != null) {
    throw new Error('Invalid argument to findOne(): ' +
      util.inspect(conditions));
  }

  prepareDiscriminatorCriteria(this);

  try {
    this.cast(this.model);
    this._castError = null;
  } catch (err) {
    this._castError = err;
  }

  if (!callback) {
    // already merged in the conditions, don't need to send them in.
    return Query.base.findOne.call(this);
  }

  this._findOne(callback);

  return this;
}
```
- example usage
```shell
...
};

/**
* Checks if 'path' was selected in the source query which initialized this document.
*
* ####Example
*
*     Thing.findOne().select('name').exec(function (err, doc) {
*        doc.isSelected('name') // true
*        doc.isSelected('age')  // false
*     })
*
* @param {String} path
* @return {Boolean}
* @api public
...
```

#### <a name="apidoc.element.mongoose.query.prototype.findOneAndRemove"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOneAndRemove (conditions, options, callback)](#apidoc.element.mongoose.query.prototype.findOneAndRemove)
- description and source-code
```javascript
findOneAndRemove = function (conditions, options, callback) {
  this.op = 'findOneAndRemove';
  this._validate();

  switch (arguments.length) {
    case 2:
      if (typeof options === 'function') {
        callback = options;
        options = {};
      }
      break;
    case 1:
      if (typeof conditions === 'function') {
        callback = conditions;
        conditions = undefined;
        options = undefined;
      }
      break;
  }

  if (mquery.canMerge(conditions)) {
    this.merge(conditions);
  }

  options && this.setOptions(options);

  if (!callback) {
    return this;
  }

  this._findOneAndRemove(callback);

  return this;
}
```
- example usage
```shell
...
*
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'maxTimeMS': puts a time limit on the query - requires mongodb >= 2.6.0
* - 'select': sets the document fields to return
*
* ####Examples:
*
*     A.findOneAndRemove(conditions, options, callback) // executes
*     A.findOneAndRemove(conditions, options)  // return Query
*     A.findOneAndRemove(conditions, callback) // executes
*     A.findOneAndRemove(conditions) // returns Query
*     A.findOneAndRemove()           // returns Query
*
* Values are cast to their appropriate types when using the findAndModify helpers.
* However, the below are never executed.
...
```

#### <a name="apidoc.element.mongoose.query.prototype.findOneAndUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>findOneAndUpdate (criteria, doc, options, callback)](#apidoc.element.mongoose.query.prototype.findOneAndUpdate)
- description and source-code
```javascript
findOneAndUpdate = function (criteria, doc, options, callback) {
  this.op = 'findOneAndUpdate';
  this._validate();

  switch (arguments.length) {
    case 3:
      if (typeof options === 'function') {
        callback = options;
        options = {};
      }
      break;
    case 2:
      if (typeof doc === 'function') {
        callback = doc;
        doc = criteria;
        criteria = undefined;
      }
      options = undefined;
      break;
    case 1:
      if (typeof criteria === 'function') {
        callback = criteria;
        criteria = options = doc = undefined;
      } else {
        doc = criteria;
        criteria = options = undefined;
      }
  }

  if (mquery.canMerge(criteria)) {
    this.merge(criteria);
  }

  // apply doc
  if (doc) {
    this._mergeUpdate(doc);
  }

  if (options) {
    options = utils.clone(options, { retainKeyOrder: true });
    if (options.projection) {
      this.select(options.projection);
      delete options.projection;
    }
    if (options.fields) {
      this.select(options.fields);
      delete options.fields;
    }

    this.setOptions(options);
  }

  if (!callback) {
    return this;
  }

  return this._findOneAndUpdate(callback);
}
```
- example usage
```shell
...
*
* Finds a matching document, updates it according to the 'update' arg, passing any 'options', and returns the found document (if
 any) to the callback. The query executes immediately if 'callback' is passed else a Query object is returned.
*
* ####Options:
*
* - 'new': bool - if true, return the modified document rather than the original. defaults to false (changed in 4.0)
* - 'upsert': bool - creates the object if it doesn't exist. defaults to false.
* - 'fields': {Object|String} - Field selection. Equivalent to '.select(fields).findOneAndUpdate()'
* - 'maxTimeMS': puts a time limit on the query - requires mongodb >= 2.6.0
* - 'sort': if multiple docs are found by the conditions, sets the sort order to choose which doc to update
* - 'runValidators': if true, runs [update validators](/docs/validation.html#update-validators) on this command. Update validators
 validate the update operation against the model's schema.
* - 'setDefaultsOnInsert': if this and 'upsert' are true, mongoose will apply the [defaults](http://mongoosejs.com/docs/defaults
.html) specified in the model's schema if a new document is created. This option only works on MongoDB >= 2.4 because it relies
on [MongoDB's '$setOnInsert' operator](https://docs.mongodb.org/v2.4/reference/operator/update/setOnInsert/).
* - 'passRawResult': if true, passes the [raw result from the MongoDB driver as the third callback parameter](http://mongodb.github
.io/node-mongodb-native/2.0/api/Collection.html#findAndModify)
*
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype.getQuery"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>getQuery ()](#apidoc.element.mongoose.query.prototype.getQuery)
- description and source-code
```javascript
getQuery = function () {
  return this._conditions;
}
```
- example usage
```shell
...
/**
 * Returns the current query conditions as a JSON object.
 *
 * ####Example:
 *
 *     var query = new Query();
 *     query.find({ a: 1 }).where('b').gt(2);
 *     query.getQuery(); // { a: 1, b: { $gt: 2 } }
 *
 * @return {Object} current query conditions
 * @api public
 */

Query.prototype.getQuery = function() {
return this._conditions;
...
```

#### <a name="apidoc.element.mongoose.query.prototype.getUpdate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>getUpdate ()](#apidoc.element.mongoose.query.prototype.getUpdate)
- description and source-code
```javascript
getUpdate = function () {
  return this._update;
}
```
- example usage
```shell
...
/**
 * Returns the current update operations as a JSON object.
 *
 * ####Example:
 *
 *     var query = new Query();
 *     query.update({}, { $set: { a: 5 } });
 *     query.getUpdate(); // { $set: { a: 5 } }
 *
 * @return {Object} current update operations
 * @api public
 */

Query.prototype.getUpdate = function() {
return this._update;
...
```

#### <a name="apidoc.element.mongoose.query.prototype.lean"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>lean (v)](#apidoc.element.mongoose.query.prototype.lean)
- description and source-code
```javascript
lean = function (v) {
  this._mongooseOptions.lean = arguments.length ? !!v : true;
  return this;
}
```
- example usage
```shell
...
*     // include all properties except for 'length'
*     Adventure.findById(id, '-length').exec(function (err, adventure) {});
*
*     // passing options (in this case return the raw js objects, not mongoose documents by passing 'lean'
*     Adventure.findById(id, 'name', { lean: true }, function (err, doc) {});
*
*     // same as above
*     Adventure.findById(id, 'name').lean().exec(function (err, doc) {});
*
* @param {Object|String|Number} id value of '_id' to query by
* @param {Object} [projection] optional fields to return (http://bit.ly/1HotzBo)
* @param {Object} [options] optional
* @param {Function} [callback]
* @return {Query}
* @see field selection #query_Query-select
...
```

#### <a name="apidoc.element.mongoose.query.prototype.maxscan"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>maxscan (v)](#apidoc.element.mongoose.query.prototype.maxscan)
- description and source-code
```javascript
maxscan = function (v) {
  this._validate(method);
  this.options[method] = v;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype.merge"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>merge (source)](#apidoc.element.mongoose.query.prototype.merge)
- description and source-code
```javascript
merge = function (source) {
  if (!source) {
    return this;
  }

  var opts = { retainKeyOrder: this.options.retainKeyOrder, overwrite: true };

  if (source instanceof Query) {
    // if source has a feature, apply it to ourselves

    if (source._conditions) {
      utils.merge(this._conditions, source._conditions, opts);
    }

    if (source._fields) {
      this._fields || (this._fields = {});
      utils.merge(this._fields, source._fields, opts);
    }

    if (source.options) {
      this.options || (this.options = {});
      utils.merge(this.options, source.options, opts);
    }

    if (source._update) {
      this._update || (this._update = {});
      utils.mergeClone(this._update, source._update);
    }

    if (source._distinct) {
      this._distinct = source._distinct;
    }

    return this;
  }

  // plain object
  utils.merge(this._conditions, source, opts);

  return this;
}
```
- example usage
```shell
...
};

if (isVirtual && virtual.options && virtual.options.options) {
  currentOptions.options = utils.clone(virtual.options.options, {
    retainKeyOrder: true
  });
}
utils.merge(currentOptions, options);
if (schema && !discriminatorKey) {
  currentOptions.model = Model;
}
options.model = Model;

available[modelName] = {
  Model: Model,
...
```

#### <a name="apidoc.element.mongoose.query.prototype.mongooseOptions"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>mongooseOptions (v)](#apidoc.element.mongoose.query.prototype.mongooseOptions)
- description and source-code
```javascript
mongooseOptions = function (v) {
  if (arguments.length > 0) {
    this._mongooseOptions = v;
  }
  return this._mongooseOptions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.query.prototype.near"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>near ()](#apidoc.element.mongoose.query.prototype.near)
- description and source-code
```javascript
near = function () {
  var params = [];
  var sphere = this._mongooseOptions.nearSphere;

  // TODO refactor

  if (arguments.length === 1) {
    if (Array.isArray(arguments[0])) {
      params.push({center: arguments[0], spherical: sphere});
    } else if (typeof arguments[0] === 'string') {
      // just passing a path
      params.push(arguments[0]);
    } else if (utils.isObject(arguments[0])) {
      if (typeof arguments[0].spherical !== 'boolean') {
        arguments[0].spherical = sphere;
      }
      params.push(arguments[0]);
    } else {
      throw new TypeError('invalid argument');
    }
  } else if (arguments.length === 2) {
    if (typeof arguments[0] === 'number' && typeof arguments[1] === 'number') {
      params.push({center: [arguments[0], arguments[1]], spherical: sphere});
    } else if (typeof arguments[0] === 'string' && Array.isArray(arguments[1])) {
      params.push(arguments[0]);
      params.push({center: arguments[1], spherical: sphere});
    } else if (typeof arguments[0] === 'string' && utils.isObject(arguments[1])) {
      params.push(arguments[0]);
      if (typeof arguments[1].spherical !== 'boolean') {
        arguments[1].spherical = sphere;
      }
      params.push(arguments[1]);
    } else {
      throw new TypeError('invalid argument');
    }
  } else if (arguments.length === 3) {
    if (typeof arguments[0] === 'string' && typeof arguments[1] === 'number'
        && typeof arguments[2] === 'number') {
      params.push(arguments[0]);
      params.push({center: [arguments[1], arguments[2]], spherical: sphere});
    } else {
      throw new TypeError('invalid argument');
    }
  } else {
    throw new TypeError('invalid argument');
  }

  return Query.base.near.apply(this, params);
}
```
- example usage
```shell
...
*
* ####NOTE:
*
* **MUST** be used as the first operator in the pipeline.
*
* ####Examples:
*
*     aggregate.near({
*       near: [40.724, -73.997],
*       distanceField: "dist.calculated", // required
*       maxDistance: 0.008,
*       query: { type: "public" },
*       includeLocs: "dist.location",
*       uniqueDocs: true,
*       num: 5
...
```

#### <a name="apidoc.element.mongoose.query.prototype.nearSphere"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>nearSphere ()](#apidoc.element.mongoose.query.prototype.nearSphere)
- description and source-code
```javascript
nearSphere = function () {
  this._mongooseOptions.nearSphere = true;
  this.near.apply(this, arguments);
  return this;
}
```
- example usage
```shell
...
};

/**
* _DEPRECATED_ Specifies a '$nearSphere' condition
*
* ####Example
*
*     query.where('loc').nearSphere({ center: [10, 10], maxDistance: 5 });
*
* **Deprecated.** Use 'query.near()' instead with the 'spherical' option set to 'true'.
*
* ####Example
*
*     query.where('loc').near({ center: [10, 10], spherical: true });
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype.populate"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>populate ()](#apidoc.element.mongoose.query.prototype.populate)
- description and source-code
```javascript
populate = function () {
  if (arguments.length === 0) {
    return this;
  }

  var res = utils.populate.apply(null, arguments);
  var opts = this._mongooseOptions;

  if (!utils.isObject(opts.populate)) {
    opts.populate = {};
  }

  var pop = opts.populate;

  for (var i = 0; i < res.length; ++i) {
    var path = res[i].path;
    if (pop[path] && pop[path].populate && res[i].populate) {
      res[i].populate = pop[path].populate.concat(res[i].populate);
    }
    pop[res[i].path] = res[i];
  }

  return this;
}
```
- example usage
```shell
...
* Populates document references, executing the 'callback' when complete.
* If you want to use promises instead, use this function with
* ['execPopulate()'](#document_Document-execPopulate)
*
* ####Example:
*
*     doc
*     .populate('company')
*     .populate({
*       path: 'notes',
*       match: /airline/,
*       select: 'text',
*       model: 'modelName'
*       options: opts
*     }, function (err, user) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype.read"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>read (pref, tags)](#apidoc.element.mongoose.query.prototype.read)
- description and source-code
```javascript
function read(pref, tags) {
  // first cast into a ReadPreference object to support tags
  var read = readPref.call(readPref, pref, tags);
  return Query.base.read.call(this, read);
}
```
- example usage
```shell
...
};

/**
* Sets the readPreference option for the aggregation query.
*
* ####Example:
*
*     Model.aggregate(..).read('primaryPreferred').exec(callback)
*
* @param {String} pref one of the listed preference options or their aliases
* @param {Array} [tags] optional tags for this query
* @see mongodb http://docs.mongodb.org/manual/applications/replication/#read-preference
* @see driver http://mongodb.github.com/node-mongodb-native/driver-articles/anintroductionto1_1and2_2.html#read-preferences
*/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.remove"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>remove (cond, callback)](#apidoc.element.mongoose.query.prototype.remove)
- description and source-code
```javascript
remove = function (cond, callback) {
  if (typeof cond === 'function') {
    callback = cond;
    cond = null;
  }

  var cb = typeof callback === 'function';

  try {
    this.cast(this.model);
  } catch (err) {
    if (cb) return process.nextTick(callback.bind(null, err));
    return this;
  }

  return Query.base.remove.call(this, cond, callback);
}
```
- example usage
```shell
...
'''

The same goes for removing them:

'''js
BlogPost.findById(myId, function (err, post) {
  if (!err) {
    post.comments[0].remove();
    post.save(function (err) {
      // do something
    });
  }
});
'''
...
```

#### <a name="apidoc.element.mongoose.query.prototype.replaceOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>replaceOne (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.replaceOne)
- description and source-code
```javascript
replaceOne = function (conditions, doc, options, callback) {
  if (typeof options === 'function') {
    // .update(conditions, doc, callback)
    callback = options;
    options = null;
  } else if (typeof doc === 'function') {
    // .update(doc, callback);
    callback = doc;
    doc = conditions;
    conditions = {};
    options = null;
  } else if (typeof conditions === 'function') {
    // .update(callback)
    callback = conditions;
    conditions = undefined;
    doc = undefined;
    options = undefined;
  } else if (typeof conditions === 'object' && !doc && !options && !callback) {
    // .update(doc)
    doc = conditions;
    conditions = undefined;
    options = undefined;
    callback = undefined;
  }

  this.setOptions({ overwrite: true });
  return _update(this, 'replaceOne', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.updateOne.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .replaceOne()
 *
 * @param {Function} callback
 * @see Model.replaceOne #model_Model.replaceOne
 * @api private
 */
Query.prototype._replaceOne = function(callback) {
var schema = this.model.schema;
...
```

#### <a name="apidoc.element.mongoose.query.prototype.setOptions"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>setOptions (options, overwrite)](#apidoc.element.mongoose.query.prototype.setOptions)
- description and source-code
```javascript
setOptions = function (options, overwrite) {
  // overwrite is only for internal use
  if (overwrite) {
    // ensure that _mongooseOptions & options are two different objects
    this._mongooseOptions = (options && utils.clone(options)) || {};
    this.options = options || {};

    if ('populate' in options) {
      this.populate(this._mongooseOptions);
    }
    return this;
  }

  if (!(options && options.constructor.name === 'Object')) {
    return this;
  }

  if (options && Array.isArray(options.populate)) {
    var populate = options.populate;
    delete options.populate;
    var _numPopulate = populate.length;
    for (var i = 0; i < _numPopulate; ++i) {
      this.populate(populate[i]);
    }
  }

  return Query.base.setOptions.call(this, options);
}
```
- example usage
```shell
...
} else if (typeof options === 'function') {
  callback = options;
  options = null;
}

var mq = new this.Query({}, {}, this, this.collection);
mq.select(projection);
mq.setOptions(options);
if (this.schema.discriminatorMapping && mq.selectedInclusively()) {
  mq.select(this.schema.options.discriminatorKey);
}

if (callback) {
  callback = this.$wrapCallback(callback);
}
...
```

#### <a name="apidoc.element.mongoose.query.prototype.sort"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>sort (arg)](#apidoc.element.mongoose.query.prototype.sort)
- description and source-code
```javascript
sort = function (arg) {
  if (arguments.length > 1) {
    throw new Error('sort() only takes 1 Argument');
  }

  return Query.base.sort.call(this, arg);
}
```
- example usage
```shell
...
* If an object is passed, values allowed are 'asc', 'desc', 'ascending', 'descending', '1', and '-1'.
*
* If a string is passed, it must be a space delimited list of path names. The sort order of each path is ascending unless the path
 name is prefixed with '-' which will be treated as descending.
*
* ####Examples:
*
*     // these are equivalent
*     aggregate.sort({ field: 'asc', test: -1 });
*     aggregate.sort('field -test');
*
* @see $sort http://docs.mongodb.org/manual/reference/aggregation/sort/
* @param {Object|String} arg
* @return {Aggregate} this
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.stream"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>stream ()](#apidoc.element.mongoose.query.prototype.stream)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
...

/**
* Returns a Node.js 0.8 style [read stream](http://nodejs.org/docs/v0.8.21/api/stream.html#stream_readable_stream) interface.
*
* ####Example
*
*     // follows the nodejs 0.8 stream api
*     Thing.find({ name: /^hello/ }).stream().pipe(res)
*
*     // manual streaming
*     var stream = Thing.find({ name: /^hello/ }).stream();
*
*     stream.on('data', function (doc) {
*       // do something with the mongoose document
*     }).on('error', function (err) {
...
```

#### <a name="apidoc.element.mongoose.query.prototype.tailable"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>tailable (val, opts)](#apidoc.element.mongoose.query.prototype.tailable)
- description and source-code
```javascript
tailable = function (val, opts) {
  // we need to support the tailable({ awaitdata : true }) as well as the
  // tailable(true, {awaitdata :true}) syntax that mquery does not support
  if (val && val.constructor.name === 'Object') {
    opts = val;
    val = true;
  }

  if (val === undefined) {
    val = true;
  }

  if (opts && typeof opts === 'object') {
    for (var key in opts) {
      if (key === 'awaitdata') {
        // For backwards compatibility
        this.options[key] = !!opts[key];
      } else {
        this.options[key] = opts[key];
      }
    }
  }

  return Query.base.tailable.call(this, val);
}
```
- example usage
```shell
...
Query.prototype.maxscan = Query.base.maxScan;

/**
* Sets the tailable option (for use with capped collections).
*
* ####Example
*
*     query.tailable() // true
*     query.tailable(true)
*     query.tailable(false)
*
* ####Note
*
* Cannot be used with 'distinct()'
*
...
```

#### <a name="apidoc.element.mongoose.query.prototype.then"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>then (resolve, reject)](#apidoc.element.mongoose.query.prototype.then)
- description and source-code
```javascript
then = function (resolve, reject) {
  return this.exec().then(resolve, reject);
}
```
- example usage
```shell
...
*
* ####Example:
*
*     aggregate.exec(callback);
*
*     // Because a promise is returned, the 'callback' is optional.
*     var promise = aggregate.exec();
*     promise.then(..);
*
* @see Promise #promise_Promise
* @param {Function} [callback]
* @return {Promise}
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.query.prototype.toConstructor"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>toConstructor ()](#apidoc.element.mongoose.query.prototype.toConstructor)
- description and source-code
```javascript
function toConstructor() {
  var model = this.model;
  var coll = this.mongooseCollection;

  var CustomQuery = function(criteria, options) {
    if (!(this instanceof CustomQuery)) {
      return new CustomQuery(criteria, options);
    }
    this._mongooseOptions = utils.clone(p._mongooseOptions);
    Query.call(this, criteria, options || null, model, coll);
  };

  util.inherits(CustomQuery, Query);

  // set inherited defaults
  var p = CustomQuery.prototype;

  p.options = {};

  p.setOptions(this.options);

  p.op = this.op;
  p._conditions = utils.clone(this._conditions, { retainKeyOrder: true });
  p._fields = utils.clone(this._fields);
  p._update = utils.clone(this._update);
  p._path = this._path;
  p._distinct = this._distinct;
  p._collection = this._collection;
  p._mongooseOptions = this._mongooseOptions;

  return CustomQuery;
}
```
- example usage
```shell
...
*
*     // Create a query for adventure movies and read from the primary
*     // node in the replica-set unless it is down, in which case we'll
*     // read from a secondary node.
*     var query = Movie.find({ tags: 'adventure' }).read('primaryPreferred');
*
*     // create a custom Query constructor based off these settings
*     var Adventure = query.toConstructor();
*
*     // Adventure is now a subclass of mongoose.Query and works the same way but with the
*     // default query parameters and options set.
*     Adventure().exec(callback)
*
*     // further narrow down our query results while still using the previous settings
*     Adventure().where({ name: /^Life/ }).exec(callback);
...
```

#### <a name="apidoc.element.mongoose.query.prototype.update"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>update (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.update)
- description and source-code
```javascript
update = function (conditions, doc, options, callback) {
  if (typeof options === 'function') {
    // .update(conditions, doc, callback)
    callback = options;
    options = null;
  } else if (typeof doc === 'function') {
    // .update(doc, callback);
    callback = doc;
    doc = conditions;
    conditions = {};
    options = null;
  } else if (typeof conditions === 'function') {
    // .update(callback)
    callback = conditions;
    conditions = undefined;
    doc = undefined;
    options = undefined;
  } else if (typeof conditions === 'object' && !doc && !options && !callback) {
    // .update(doc)
    doc = conditions;
    conditions = undefined;
    options = undefined;
    callback = undefined;
  }

  return _update(this, 'update', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

/**
* Sends an update command with this document '_id' as the query selector.
*
* ####Example:
*
*     weirdCar.update({$inc: {wheels:1}}, { w: 1 }, callback);
*
* ####Valid options:
*
*  - same as in [Model.update](#model_Model.update)
*
* @see Model.update #model_Model.update
* @param {Object} doc
...
```

#### <a name="apidoc.element.mongoose.query.prototype.updateMany"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>updateMany (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.updateMany)
- description and source-code
```javascript
updateMany = function (conditions, doc, options, callback) {
  if (typeof options === 'function') {
    // .update(conditions, doc, callback)
    callback = options;
    options = null;
  } else if (typeof doc === 'function') {
    // .update(doc, callback);
    callback = doc;
    doc = conditions;
    conditions = {};
    options = null;
  } else if (typeof conditions === 'function') {
    // .update(callback)
    callback = conditions;
    conditions = undefined;
    doc = undefined;
    options = undefined;
  } else if (typeof conditions === 'object' && !doc && !options && !callback) {
    // .update(doc)
    doc = conditions;
    conditions = undefined;
    options = undefined;
    callback = undefined;
  }

  return _update(this, 'updateMany', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.update.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .updateMany()
 *
 * @param {Function} callback
 * @see Model.update #model_Model.update
 * @api private
 */
Query.prototype._updateMany = function(callback) {
var schema = this.model.schema;
...
```

#### <a name="apidoc.element.mongoose.query.prototype.updateOne"></a>[function <span class="apidocSignatureSpan">mongoose.query.prototype.</span>updateOne (conditions, doc, options, callback)](#apidoc.element.mongoose.query.prototype.updateOne)
- description and source-code
```javascript
updateOne = function (conditions, doc, options, callback) {
  if (typeof options === 'function') {
    // .update(conditions, doc, callback)
    callback = options;
    options = null;
  } else if (typeof doc === 'function') {
    // .update(doc, callback);
    callback = doc;
    doc = conditions;
    conditions = {};
    options = null;
  } else if (typeof conditions === 'function') {
    // .update(callback)
    callback = conditions;
    conditions = undefined;
    doc = undefined;
    options = undefined;
  } else if (typeof conditions === 'object' && !doc && !options && !callback) {
    // .update(doc)
    doc = conditions;
    conditions = undefined;
    options = undefined;
    callback = undefined;
  }

  return _update(this, 'updateOne', conditions, doc, options, callback);
}
```
- example usage
```shell
...
}

Query.base.updateMany.call(this, castedQuery, castedDoc, options, callback);
return this;
};

/*!
 * Internal thunk for .updateOne()
 *
 * @param {Function} callback
 * @see Model.update #model_Model.update
 * @api private
 */
Query.prototype._updateOne = function(callback) {
var schema = this.model.schema;
...
```



# <a name="apidoc.module.mongoose.querycursor"></a>[module mongoose.querycursor](#apidoc.module.mongoose.querycursor)

#### <a name="apidoc.element.mongoose.querycursor.querycursor"></a>[function <span class="apidocSignatureSpan">mongoose.</span>querycursor (query, options)](#apidoc.element.mongoose.querycursor.querycursor)
- description and source-code
```javascript
function QueryCursor(query, options) {
  Readable.call(this, { objectMode: true });

  this.cursor = null;
  this.query = query;
  this._transforms = options.transform ? [options.transform] : [];
  var _this = this;
  var model = query.model;
  model.collection.find(query._conditions, options, function(err, cursor) {
    if (_this._error) {
      cursor.close(function() {});
      _this.listeners('error').length > 0 && _this.emit('error', _this._error);
    }
    if (err) {
      return _this.emit('error', err);
    }
    _this.cursor = cursor;
    _this.emit('cursor', cursor);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querycursor.super_"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.</span>super_ (options)](#apidoc.element.mongoose.querycursor.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.querycursor.prototype"></a>[module mongoose.querycursor.prototype](#apidoc.module.mongoose.querycursor.prototype)

#### <a name="apidoc.element.mongoose.querycursor.prototype._markError"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>_markError (error)](#apidoc.element.mongoose.querycursor.prototype._markError)
- description and source-code
```javascript
_markError = function (error) {
  this._error = error;
  return this;
}
```
- example usage
```shell
...
  if (opts) {
    this.setOptions(opts);
  }

  try {
    this.cast(this.model);
  } catch (err) {
    return (new QueryCursor(this, this.options))._markError(err);
  }

  return new QueryCursor(this, this.options);
};

// the rest of these are basically to support older Mongoose syntax with mquery
...
```

#### <a name="apidoc.element.mongoose.querycursor.prototype._read"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>_read ()](#apidoc.element.mongoose.querycursor.prototype._read)
- description and source-code
```javascript
_read = function () {
  var _this = this;
  _next(this, function(error, doc) {
    if (error) {
      return _this.emit('error', error);
    }
    if (!doc) {
      _this.push(null);
      _this.cursor.close(function(error) {
        if (error) {
          return _this.emit('error', error);
        }
        setTimeout(function() {
          _this.emit('close');
        }, 0);
      });
      return;
    }
    _this.push(doc);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querycursor.prototype.close"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>close (callback)](#apidoc.element.mongoose.querycursor.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  var Promise = PromiseProvider.get();
  var _this = this;
  return new Promise.ES6(function(resolve, reject) {
    _this.cursor.close(function(error) {
      if (error) {
        callback && callback(error);
        reject(error);
        return _this.listeners('error').length > 0 &&
          _this.emit('error', error);
      }
      _this.emit('close');
      resolve();
      callback && callback();
    });
  });
}
```
- example usage
```shell
...
* For practical reasons, a Connection equals a Db.
*
* @param {Mongoose} base a mongoose instance
* @inherits NodeJS EventEmitter http://nodejs.org/api/events.html#events_class_events_eventemitter
* @event 'connecting': Emitted when 'connection.{open,openSet}()' is executed on this connection.
* @event 'connected': Emitted when this connection successfully connects to the db. May be emitted _multiple_ times in 'reconnected
' scenarios.
* @event 'open': Emitted after we 'connected' and 'onOpen' is executed on all of this connections models.
* @event 'disconnecting': Emitted when 'connection.close()' was executed.
* @event 'disconnected': Emitted after getting disconnected from the db.
* @event 'close': Emitted after we 'disconnected' and 'onClose' executed on all of this connections models.
* @event 'reconnected': Emitted after we 'connected' and subsequently 'disconnected', followed by successfully another successfull
 connection.
* @event 'error': Emitted when an error occurs on this connection.
* @event 'fullsetup': Emitted in a replica-set scenario, when primary and at least one seconaries specified in the connection string
 are connected.
* @event 'all': Emitted in a replica-set scenario, when all nodes specified in the connection string are connected.
* @api public
...
```

#### <a name="apidoc.element.mongoose.querycursor.prototype.eachAsync"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>eachAsync (fn, callback)](#apidoc.element.mongoose.querycursor.prototype.eachAsync)
- description and source-code
```javascript
eachAsync = function (fn, callback) {
  var Promise = PromiseProvider.get();
  var _this = this;

  var handleNextResult = function(doc, callback) {
    var promise = fn(doc);
    if (promise && typeof promise.then === 'function') {
      promise.then(
        function() { callback(null); },
        function(error) { callback(error); });
    } else {
      callback(null);
    }
  };

  var iterate = function(callback) {
    return _next(_this, function(error, doc) {
      if (error) {
        return callback(error);
      }
      if (!doc) {
        return callback(null);
      }
      handleNextResult(doc, function(error) {
        if (error) {
          return callback(error);
        }
        // Make sure to clear the stack re: gh-4697
        setTimeout(function() {
          iterate(callback);
        }, 0);
      });
    });
  };

  return new Promise.ES6(function(resolve, reject) {
    iterate(function(error) {
      if (error) {
        callback && callback(error);
        return reject(error);
      }
      callback && callback(null);
      return resolve();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querycursor.prototype.map"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>map (fn)](#apidoc.element.mongoose.querycursor.prototype.map)
- description and source-code
```javascript
map = function (fn) {
  this._transforms.push(fn);
  return this;
}
```
- example usage
```shell
...
    val.length > 0 &&
    val[0] instanceof Document &&
    val[0].constructor.modelName &&
    (schema.options.type[0].ref === val[0].constructor.baseModelName || schema.options.type[0].ref === val[0].constructor.modelName
)) {
  if (this.ownerDocument) {
    popOpts = { model: val[0].constructor };
    this.ownerDocument().populated(this.$__fullPath(path),
      val.map(function(v) { return v._id; }), popOpts);
  } else {
    popOpts = { model: val[0].constructor };
    this.populated(path, val.map(function(v) { return v._id; }), popOpts);
  }
  didPopulate = true;
}
val = schema.applySetters(val, this, false, priorVal);
...
```

#### <a name="apidoc.element.mongoose.querycursor.prototype.next"></a>[function <span class="apidocSignatureSpan">mongoose.querycursor.prototype.</span>next (callback)](#apidoc.element.mongoose.querycursor.prototype.next)
- description and source-code
```javascript
next = function (callback) {
  var Promise = PromiseProvider.get();
  var _this = this;
  return new Promise.ES6(function(resolve, reject) {
    _next(_this, function(error, doc) {
      if (error) {
        callback && callback(error);
        return reject(error);
      }
      callback && callback(null, doc);
      resolve(doc);
    });
  });
}
```
- example usage
```shell
...
      function(error) { callback(error); });
  } else {
    callback(null);
  }
};

var iterate = function(callback) {
  return cursor.next(function(error, doc) {
    if (error) {
      return callback(error);
    }
    if (!doc) {
      return callback(null);
    }
    handleNextResult(doc, function(error) {
...
```



# <a name="apidoc.module.mongoose.queryhelpers"></a>[module mongoose.queryhelpers](#apidoc.module.mongoose.queryhelpers)

#### <a name="apidoc.element.mongoose.queryhelpers.applyPaths"></a>[function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>applyPaths (fields, schema)](#apidoc.element.mongoose.queryhelpers.applyPaths)
- description and source-code
```javascript
function applyPaths(fields, schema) {
  // determine if query is selecting or excluding fields

  var exclude;
  var keys;
  var ki;

  if (fields) {
    keys = Object.keys(fields);
    ki = keys.length;

    while (ki--) {
      if (keys[ki][0] === '+') continue;
      exclude = fields[keys[ki]] === 0;
      break;
    }
  }

  // if selecting, apply default schematype select:true fields
  // if excluding, apply schematype select:false fields

  var selected = [],
      excluded = [],
      seen = [];

  var analyzePath = function(path, type) {
    if (typeof type.selected !== 'boolean') return;

    var plusPath = '+' + path;
    if (fields && plusPath in fields) {
      // forced inclusion
      delete fields[plusPath];

      // if there are other fields being included, add this one
      // if no other included fields, leave this out (implied inclusion)
      if (exclude === false && keys.length > 1 && !~keys.indexOf(path)) {
        fields[path] = 1;
      }

      return;
    }

    // check for parent exclusions
    var root = path.split('.')[0];
    if (~excluded.indexOf(root)) return;

    (type.selected ? selected : excluded).push(path);
  };

  var analyzeSchema = function(schema, prefix) {
    prefix || (prefix = '');

    // avoid recursion
    if (~seen.indexOf(schema)) return;
    seen.push(schema);

    schema.eachPath(function(path, type) {
      if (prefix) path = prefix + '.' + path;

      analyzePath(path, type);

      // array of subdocs?
      if (type.schema) {
        analyzeSchema(type.schema, path);
      }
    });
  };

  analyzeSchema(schema);

  var i;
  switch (exclude) {
    case true:
      for (i = 0; i < excluded.length; ++i) {
        fields[excluded[i]] = 0;
      }
      break;
    case false:
      if (schema &&
          schema.paths['_id'] &&
          schema.paths['_id'].options &&
          schema.paths['_id'].options.select === false) {
        fields._id = 0;
      }
      for (i = 0; i < selected.length; ++i) {
        fields[selected[i]] = 1;
      }
      break;
    case undefined:
      // user didn't specify fields, implies returning all fields.
      // only need to apply excluded fields
      for (i = 0; i < excluded.length; ++i) {
        fields[excluded[i]] = 0;
      }
      break;
  }
}
```
- example usage
```shell
...
/**
* Applies schematype selected options to this query.
* @api private
*/

Query.prototype._applyPaths = function applyPaths() {
 this._fields = this._fields || {};
 helpers.applyPaths(this._fields, this.model.schema);
};

/**
* Returns a Node.js 0.8 style [read stream](http://nodejs.org/docs/v0.8.21/api/stream.html#stream_readable_stream) interface.
*
* ####Example
*
...
```

#### <a name="apidoc.element.mongoose.queryhelpers.createModel"></a>[function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>createModel (model, doc, fields)](#apidoc.element.mongoose.queryhelpers.createModel)
- description and source-code
```javascript
function createModel(model, doc, fields) {
  var discriminatorMapping = model.schema
    ? model.schema.discriminatorMapping
    : null;

  var key = discriminatorMapping && discriminatorMapping.isRoot
    ? discriminatorMapping.key
    : null;

  if (key && doc[key] && model.discriminators && model.discriminators[doc[key]]) {
    var discriminator = model.discriminators[doc[key]];
    var _fields = utils.clone(fields);
    exports.applyPaths(_fields, discriminator.schema);
    return new model.discriminators[doc[key]](undefined, _fields, true);
  }

  return new model(undefined, fields, true);
}
```
- example usage
```shell
...
*
* @param {Object} obj
* @return {Document}
* @api public
*/

Model.hydrate = function(obj) {
 var model = require('./queryhelpers').createModel(this, obj);
 model.init(obj);
 return model;
};

/**
* Updates documents in the database without returning them.
*
...
```

#### <a name="apidoc.element.mongoose.queryhelpers.preparePopulationOptions"></a>[function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>preparePopulationOptions (query, options)](#apidoc.element.mongoose.queryhelpers.preparePopulationOptions)
- description and source-code
```javascript
function preparePopulationOptions(query, options) {
  var pop = utils.object.vals(query.options.populate);

  // lean options should trickle through all queries
  if (options.lean) pop.forEach(makeLean);

  return pop;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.queryhelpers.preparePopulationOptionsMQ"></a>[function <span class="apidocSignatureSpan">mongoose.queryhelpers.</span>preparePopulationOptionsMQ (query, options)](#apidoc.element.mongoose.queryhelpers.preparePopulationOptionsMQ)
- description and source-code
```javascript
function preparePopulationOptionsMQ(query, options) {
  var pop = utils.object.vals(query._mongooseOptions.populate);

  // lean options should trickle through all queries
  if (options.lean) pop.forEach(makeLean);

  return pop;
}
```
- example usage
```shell
...

if (!options.populate) {
  return options.lean === true
      ? callback(null, docs)
      : completeMany(_this.model, docs, fields, null, callback);
}

var pop = helpers.preparePopulationOptionsMQ(_this, options);
pop.__noPromise = true;
_this.model.populate(docs, pop, function(err, docs) {
  if (err) return callback(err);
  return options.lean === true
      ? callback(null, docs)
      : completeMany(_this.model, docs, fields, pop, callback);
});
...
```



# <a name="apidoc.module.mongoose.querystream"></a>[module mongoose.querystream](#apidoc.module.mongoose.querystream)

#### <a name="apidoc.element.mongoose.querystream.querystream"></a>[function <span class="apidocSignatureSpan">mongoose.</span>querystream (query, options)](#apidoc.element.mongoose.querystream.querystream)
- description and source-code
```javascript
function QueryStream(query, options) {
  Stream.call(this);

  this.query = query;
  this.readable = true;
  this.paused = false;
  this._cursor = null;
  this._destroyed = null;
  this._fields = null;
  this._buffer = null;
  this._inline = T_INIT;
  this._running = false;
  this._transform = options && typeof options.transform === 'function'
      ? options.transform
      : K;

  // give time to hook up events
  var _this = this;
  process.nextTick(function() {
    _this._init();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.querystream.prototype"></a>[module mongoose.querystream.prototype](#apidoc.module.mongoose.querystream.prototype)

#### <a name="apidoc.element.mongoose.querystream.prototype.__next"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>__next ()](#apidoc.element.mongoose.querystream.prototype.__next)
- description and source-code
```javascript
__next = function () {
  if (this.paused || this._destroyed) {
    this._running = false;
    return this._running;
  }

  var _this = this;
  _this._inline = T_INIT;

  _this._cursor.nextObject(function cursorcb(err, doc) {
    _this._onNextObject(err, doc);
  });

  // if onNextObject() was already called in this tick
  // return ourselves to the trampoline.
  if (T_CONT === this._inline) {
    return true;
  }
  // onNextObject() hasn't fired yet. tell onNextObject
  // that its ok to call _next b/c we are not within
  // the trampoline anymore.
  this._inline = T_IDLE;
}
```
- example usage
```shell
...
   while (!this.paused && !this._destroyed && (arg = this._buffer.shift())) { // eslint-disable-line no-cond-assign
     this._onNextObject.apply(this, arg);
   }
 }

 // avoid stack overflows with large result sets.
 // trampoline instead of recursion.
 while (this.__next()) {
 }
};

/**
* Pulls the next doc from the cursor.
*
* @see QueryStream#_next #querystream_QueryStream-_next
...
```

#### <a name="apidoc.element.mongoose.querystream.prototype._init"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_init ()](#apidoc.element.mongoose.querystream.prototype._init)
- description and source-code
```javascript
_init = function () {
  if (this._destroyed) {
    return;
  }

  var query = this.query,
      model = query.model,
      options = query._optionsForExec(model),
      _this = this;

  try {
    query.cast(model);
  } catch (err) {
    return _this.destroy(err);
  }

  _this._fields = utils.clone(query._fields);
  options.fields = query._castFields(_this._fields);

  model.collection.find(query._conditions, options, function(err, cursor) {
    if (err) {
      return _this.destroy(err);
    }
    _this._cursor = cursor;
    _this._next();
  });
}
```
- example usage
```shell
...
 this._transform = options && typeof options.transform === 'function'
     ? options.transform
     : K;

 // give time to hook up events
 var _this = this;
 process.nextTick(function() {
   _this._init();
 });
}

/*!
* Inherit from Stream
*/
...
```

#### <a name="apidoc.element.mongoose.querystream.prototype._next"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_next ()](#apidoc.element.mongoose.querystream.prototype._next)
- description and source-code
```javascript
function _next() {
  if (this.paused || this._destroyed) {
    this._running = false;
    return this._running;
  }

  this._running = true;

  if (this._buffer && this._buffer.length) {
    var arg;
    while (!this.paused && !this._destroyed && (arg = this._buffer.shift())) { // eslint-disable-line no-cond-assign
      this._onNextObject.apply(this, arg);
    }
  }

  // avoid stack overflows with large result sets.
  // trampoline instead of recursion.
  while (this.__next()) {
  }
}
```
- example usage
```shell
...
 options.fields = query._castFields(_this._fields);

 model.collection.find(query._conditions, options, function(err, cursor) {
   if (err) {
     return _this.destroy(err);
   }
   _this._cursor = cursor;
   _this._next();
 });
};

/**
* Trampoline for pulling the next doc from cursor.
*
* @see QueryStream#__next #querystream_QueryStream-__next
...
```

#### <a name="apidoc.element.mongoose.querystream.prototype._onNextObject"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>_onNextObject (err, doc)](#apidoc.element.mongoose.querystream.prototype._onNextObject)
- description and source-code
```javascript
function _onNextObject(err, doc) {
  if (this._destroyed) {
    return;
  }

  if (this.paused) {
    this._buffer || (this._buffer = []);
    this._buffer.push([err, doc]);
    this._running = false;
    return this._running;
  }

  if (err) {
    return this.destroy(err);
  }

  // when doc is null we hit the end of the cursor
  if (!doc) {
    this.emit('end');
    return this.destroy();
  }

  var opts = this.query._mongooseOptions;

  if (!opts.populate) {
    return opts.lean === true ?
        emit(this, doc) :
        createAndEmit(this, null, doc);
  }

  var _this = this;
  var pop = helpers.preparePopulationOptionsMQ(_this.query, _this.query._mongooseOptions);

  // Hack to work around gh-3108
  pop.forEach(function(option) {
    delete option.model;
  });

  pop.__noPromise = true;
  _this.query.model.populate(doc, pop, function(err, doc) {
    if (err) {
      return _this.destroy(err);
    }
    return opts.lean === true ?
        emit(_this, doc) :
        createAndEmit(_this, pop, doc);
  });
}
```
- example usage
```shell
...
  return this._running;
}

var _this = this;
_this._inline = T_INIT;

_this._cursor.nextObject(function cursorcb(err, doc) {
  _this._onNextObject(err, doc);
});

// if onNextObject() was already called in this tick
// return ourselves to the trampoline.
if (T_CONT === this._inline) {
  return true;
}
...
```

#### <a name="apidoc.element.mongoose.querystream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>destroy (err)](#apidoc.element.mongoose.querystream.prototype.destroy)
- description and source-code
```javascript
destroy = function (err) {
  if (this._destroyed) {
    return;
  }
  this._destroyed = true;
  this._running = false;
  this.readable = false;

  if (this._cursor) {
    this._cursor.close();
  }

  if (err) {
    this.emit('error', err);
  }

  this.emit('close');
}
```
- example usage
```shell
...
    model = query.model,
    options = query._optionsForExec(model),
    _this = this;

try {
  query.cast(model);
} catch (err) {
  return _this.destroy(err);
}

_this._fields = utils.clone(query._fields);
options.fields = query._castFields(_this._fields);

model.collection.find(query._conditions, options, function(err, cursor) {
  if (err) {
...
```

#### <a name="apidoc.element.mongoose.querystream.prototype.pause"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>pause ()](#apidoc.element.mongoose.querystream.prototype.pause)
- description and source-code
```javascript
pause = function () {
  this.paused = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.querystream.prototype.resume"></a>[function <span class="apidocSignatureSpan">mongoose.querystream.prototype.</span>resume ()](#apidoc.element.mongoose.querystream.prototype.resume)
- description and source-code
```javascript
resume = function () {
  this.paused = false;

  if (!this._cursor) {
    // cannot start if not initialized
    return;
  }

  // are we within the trampoline?
  if (T_INIT === this._inline) {
    return;
  }

  if (!this._running) {
    // outside QueryStream control, need manual restart
    return this._next();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.schema"></a>[module mongoose.schema](#apidoc.module.mongoose.schema)

#### <a name="apidoc.element.mongoose.schema.schema"></a>[function <span class="apidocSignatureSpan">mongoose.</span>schema (obj, options)](#apidoc.element.mongoose.schema.schema)
- description and source-code
```javascript
function Schema(obj, options) {
  if (!(this instanceof Schema)) {
    return new Schema(obj, options);
  }

  this.obj = obj;
  this.paths = {};
  this.subpaths = {};
  this.virtuals = {};
  this.singleNestedPaths = {};
  this.nested = {};
  this.inherits = {};
  this.callQueue = [];
  this._indexes = [];
  this.methods = {};
  this.statics = {};
  this.tree = {};
  this.query = {};
  this.childSchemas = [];

  this.s = {
    hooks: new Kareem(),
    kareemHooks: IS_KAREEM_HOOK
  };

  this.options = this.defaultOptions(options);

  // build paths
  if (obj) {
    this.add(obj);
  }

  // check if _id's value is a subdocument (gh-2276)
  var _idSubDoc = obj && obj._id && utils.isObject(obj._id);

  // ensure the documents get an auto _id unless disabled
  var auto_id = !this.paths['_id'] &&
      (!this.options.noId && this.options._id) && !_idSubDoc;

  if (auto_id) {
    obj = {_id: {auto: true}};
    obj._id[this.options.typeKey] = Schema.ObjectId;
    this.add(obj);
  }

  // ensure the documents receive an id getter unless disabled
  var autoid = !this.paths['id'] &&
      (!this.options.noVirtualId && this.options.id);
  if (autoid) {
    this.virtual('id').get(idGetter);
  }

  for (var i = 0; i < this._defaultMiddleware.length; ++i) {
    var m = this._defaultMiddleware[i];
    this[m.kind](m.hook, !!m.isAsync, m.fn);
  }

  if (this.options.timestamps) {
    this.setupTimestamp(this.options.timestamps);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.ObjectId"></a>[function <span class="apidocSignatureSpan">mongoose.schema.</span>ObjectId (key, options)](#apidoc.element.mongoose.schema.ObjectId)
- description and source-code
```javascript
function ObjectId(key, options) {
  SchemaType.call(this, key, options, 'ObjectID');
}
```
- example usage
```shell
...
*     .unwind('tags')
*     .exec(callback)
*
* ####Note:
*
* - The documents returned are plain javascript objects, not mongoose documents (since any shape of document can be returned).
* - Requires MongoDB >= 2.1
* - Mongoose does **not** cast pipeline stages. 'new Aggregate({ $match: { _id: '00000000000000000000000a' } });' will not work
unless '_id' is a string in the database. Use 'new Aggregate({ $match: { _id: mongoose.Types.ObjectId('00000000000000000000000a') } });'
instead.
*
* @see MongoDB http://docs.mongodb.org/manual/applications/aggregation/
* @see driver http://mongodb.github.com/node-mongodb-native/api-generated/collection.html#aggregate
* @param {Object|Array} [ops] aggregation operator(s) or operator array
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.schema.interpretAsType"></a>[function <span class="apidocSignatureSpan">mongoose.schema.</span>interpretAsType (path, obj, options)](#apidoc.element.mongoose.schema.interpretAsType)
- description and source-code
```javascript
interpretAsType = function (path, obj, options) {
  if (obj.constructor) {
    var constructorName = utils.getFunctionName(obj.constructor);
    if (constructorName !== 'Object') {
      var oldObj = obj;
      obj = {};
      obj[options.typeKey] = oldObj;
    }
  }

  // Get the type making sure to allow keys named "type"
  // and default to mixed if not specified.
  // { type: { type: String, default: 'freshcut' } }
  var type = obj[options.typeKey] && (options.typeKey !== 'type' || !obj.type.type)
      ? obj[options.typeKey]
      : {};

  if (utils.getFunctionName(type.constructor) === 'Object' || type === 'mixed') {
    return new MongooseTypes.Mixed(path, obj);
  }

  if (Array.isArray(type) || Array === type || type === 'array') {
    // if it was specified through { type } look for 'cast'
    var cast = (Array === type || type === 'array')
        ? obj.cast
        : type[0];

    if (cast && cast.instanceOfSchema) {
      return new MongooseTypes.DocumentArray(path, cast, obj);
    }

    if (Array.isArray(cast)) {
      return new MongooseTypes.Array(path, Schema.interpretAsType(path, cast, options), obj);
    }

    if (typeof cast === 'string') {
      cast = MongooseTypes[cast.charAt(0).toUpperCase() + cast.substring(1)];
    } else if (cast && (!cast[options.typeKey] || (options.typeKey === 'type' && cast.type.type))
        && utils.getFunctionName(cast.constructor) === 'Object') {
      if (Object.keys(cast).length) {
        // The 'minimize' and 'typeKey' options propagate to child schemas
        // declared inline, like '{ arr: [{ val: { $type: String } }] }'.
        // See gh-3560
        var childSchemaOptions = {minimize: options.minimize};
        if (options.typeKey) {
          childSchemaOptions.typeKey = options.typeKey;
        }
        //propagate 'strict' option to child schema
        if (options.hasOwnProperty('strict')) {
          childSchemaOptions.strict = options.strict;
        }
        var childSchema = new Schema(cast, childSchemaOptions);
        childSchema.$implicitlyCreated = true;
        return new MongooseTypes.DocumentArray(path, childSchema, obj);
      } else {
        // Special case: empty object becomes mixed
        return new MongooseTypes.Array(path, MongooseTypes.Mixed, obj);
      }
    }

    if (cast) {
      type = cast[options.typeKey] && (options.typeKey !== 'type' || !cast.type.type)
          ? cast[options.typeKey]
          : cast;

      name = typeof type === 'string'
          ? type
          : type.schemaName || utils.getFunctionName(type);

      if (!(name in MongooseTypes)) {
        throw new TypeError('Undefined type '' + name + '' at array '' + path +
          ''');
      }
    }

    return new MongooseTypes.Array(path, cast || MongooseTypes.Mixed, obj, options);
  }

  if (type && type.instanceOfSchema) {
    return new MongooseTypes.Embedded(type, path, obj);
  }

  var name;
  if (Buffer.isBuffer(type)) {
    name = 'Buffer';
  } else {
    name = typeof type === 'string'
        ? type
      // If not string, 'type' is a function. Outside of IE, function.name
      // gives you the function name. In IE, you need to compute it
        : type.schemaName || utils.getFunctionName(type);
  }

  if (name) {
    name = name.charAt(0).toUpperCase() + name.substring(1);
  }

  if (undefined == MongooseTypes[name]) {
    throw new TypeError('Undefined type '' + name + '' at '' + path +
        ''\n  Did you try nesting Schemas? ' +
        'You can only nest using refs or arrays.');
  }

  return new MongooseTypes[name](path, obj);
}
```
- example usage
```shell
...

  var strict = options && 'strict' in options
  ? options.strict
  : this.$__.strictMode;

  if (adhoc) {
adhocs = this.$__.adhocPaths || (this.$__.adhocPaths = {});
adhocs[path] = Schema.interpretAsType(path, type, this.schema.options);
  }

  if (typeof path !== 'string') {
// new Document({ key: val })

if (path === null || path === void 0) {
  var _ = path;
...
```



# <a name="apidoc.module.mongoose.schema.prototype"></a>[module mongoose.schema.prototype](#apidoc.module.mongoose.schema.prototype)

#### <a name="apidoc.element.mongoose.schema.prototype._getPathType"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getPathType (path)](#apidoc.element.mongoose.schema.prototype._getPathType)
- description and source-code
```javascript
_getPathType = function (path) {
  var _this = this;
  var pathschema = _this.path(path);

  if (pathschema) {
    return 'real';
  }

  function search(parts, schema) {
    var p = parts.length + 1,
        foundschema,
        trypath;

    while (p--) {
      trypath = parts.slice(0, p).join('.');
      foundschema = schema.path(trypath);
      if (foundschema) {
        if (foundschema.caster) {
          // array of Mixed?
          if (foundschema.caster instanceof MongooseTypes.Mixed) {
            return { schema: foundschema, pathType: 'mixed' };
          }

          // Now that we found the array, we need to check if there
          // are remaining document paths to look up for casting.
          // Also we need to handle array.$.path since schema.path
          // doesn't work for that.
          // If there is no foundschema.schema we are dealing with
          // a path like array.$
          if (p !== parts.length && foundschema.schema) {
            if (parts[p] === '$') {
              if (p === parts.length - 1) {
                return { schema: foundschema, pathType: 'nested' };
              }
              // comments.$.comments.$.title
              return search(parts.slice(p + 1), foundschema.schema);
            }
            // this is the last path of the selector
            return search(parts.slice(p), foundschema.schema);
          }
          return {
            schema: foundschema,
            pathType: foundschema.$isSingleNested ? 'nested' : 'array'
          };
        }
        return { schema: foundschema, pathType: 'real' };
      } else if (p === parts.length && schema.nested[trypath]) {
        return { schema: schema, pathType: 'nested' };
      }
    }
    return { schema: foundschema || schema, pathType: 'undefined' };
  }

  // look for arrays
  return search(path.split('.'), _this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype._getSchema"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getSchema (path)](#apidoc.element.mongoose.schema.prototype._getSchema)
- description and source-code
```javascript
_getSchema = function (path) {
  var _this = this;
  var pathschema = _this.path(path);
  var resultPath = [];

  if (pathschema) {
    pathschema.$fullPath = path;
    return pathschema;
  }

  function search(parts, schema) {
    var p = parts.length + 1,
        foundschema,
        trypath;

    while (p--) {
      trypath = parts.slice(0, p).join('.');
      foundschema = schema.path(trypath);
      if (foundschema) {
        resultPath.push(trypath);

        if (foundschema.caster) {
          // array of Mixed?
          if (foundschema.caster instanceof MongooseTypes.Mixed) {
            foundschema.caster.$fullPath = resultPath.join('.');
            return foundschema.caster;
          }

          // Now that we found the array, we need to check if there
          // are remaining document paths to look up for casting.
          // Also we need to handle array.$.path since schema.path
          // doesn't work for that.
          // If there is no foundschema.schema we are dealing with
          // a path like array.$
          if (p !== parts.length && foundschema.schema) {
            var ret;
            if (parts[p] === '$') {
              // comments.$.comments.$.title
              ret = search(parts.slice(p + 1), foundschema.schema);
              if (ret) {
                ret.$isUnderneathDocArray = ret.$isUnderneathDocArray ||
                  !foundschema.schema.$isSingleNested;
              }
              return ret;
            }
            // this is the last path of the selector
            ret = search(parts.slice(p), foundschema.schema);
            if (ret) {
              ret.$isUnderneathDocArray = ret.$isUnderneathDocArray ||
                !foundschema.schema.$isSingleNested;
            }
            return ret;
          }
        }

        foundschema.$fullPath = resultPath.join('.');

        return foundschema;
      }
    }
  }

  // look for arrays
  return search(path.split('.'), _this);
}
```
- example usage
```shell
...
    map = [],
    modelNameFromQuery = options.model && options.model.modelName || options.model,
    schema, refPath, Model, currentOptions, modelNames, modelName, discriminatorKey, modelForFindSchema;

var originalOptions = utils.clone(options);
var isVirtual = false;

schema = model._getSchema(options.path);
var isUnderneathDocArray = schema && schema.$isUnderneathDocArray;
if (isUnderneathDocArray &&
    originalOptions &&
    originalOptions.options &&
    originalOptions.options.sort) {
  return new Error('Cannot populate with 'sort' on path ' + options.path +
    ' because it is a subproperty of a document array');
...
```

#### <a name="apidoc.element.mongoose.schema.prototype._getVirtual"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>_getVirtual (name)](#apidoc.element.mongoose.schema.prototype._getVirtual)
- description and source-code
```javascript
_getVirtual = function (name) {
  return _getVirtual(this, name);
}
```
- example usage
```shell
...

  function setValue(val) {
return valueFilter(val, options);
  }

  for (var i = 0; i < docs.length; ++i) {
if (utils.getValue(o.path, docs[i]) == null &&
  !o.originalModel.schema._getVirtual(o.path)) {
  continue;
}

if (o.isVirtual && !o.justOne && !Array.isArray(rawIds[i])) {
  rawIds[i] = [rawIds[i]];
}
utils.setValue(o.path, rawIds[i], docs[i], setValue);
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.add"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>add (obj, prefix)](#apidoc.element.mongoose.schema.prototype.add)
- description and source-code
```javascript
function add(obj, prefix) {
  prefix = prefix || '';
  var keys = Object.keys(obj);

  for (var i = 0; i < keys.length; ++i) {
    var key = keys[i];

    if (obj[key] == null) {
      throw new TypeError('Invalid value for schema path '' + prefix + key + ''');
    }

    if (Array.isArray(obj[key]) && obj[key].length === 1 && obj[key][0] == null) {
      throw new TypeError('Invalid value for schema Array path '' + prefix + key + ''');
    }

    if (utils.isObject(obj[key]) &&
        (!obj[key].constructor || utils.getFunctionName(obj[key].constructor) === 'Object') &&
        (!obj[key][this.options.typeKey] || (this.options.typeKey === 'type' && obj[key].type.type))) {
      if (Object.keys(obj[key]).length) {
        // nested object { last: { name: String }}
        this.nested[prefix + key] = true;
        this.add(obj[key], prefix + key + '.');
      } else {
        if (prefix) {
          this.nested[prefix.substr(0, prefix.length - 1)] = true;
        }
        this.path(prefix + key, obj[key]); // mixed type
      }
    } else {
      if (prefix) {
        this.nested[prefix.substr(0, prefix.length - 1)] = true;
      }
      this.path(prefix + key, obj[key]);
    }
  }
}
```
- example usage
```shell
...
* Adds a discriminator type.
*
* ####Example:
*
*     function BaseSchema() {
*       Schema.apply(this, arguments);
*
*       this.add({
*         name: String,
*         createdAt: Date
*       });
*     }
*     util.inherits(BaseSchema, Schema);
*
*     var PersonSchema = new BaseSchema();
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.clone"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>clone ()](#apidoc.element.mongoose.schema.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var s = Object.create(Schema.prototype);
  utils.merge(s, this, { retainKeyOrder: true, hasOwnProperty: true });
  return s;
}
```
- example usage
```shell
...

Aggregate.prototype.exec = function(callback) {
if (!this._model) {
  throw new Error('Aggregate not bound to any Model');
}
var _this = this;
var Promise = PromiseProvider.get();
var options = utils.clone(this.options);

if (options && options.cursor) {
  if (options.cursor.async) {
    delete options.cursor.async;
    return new Promise.ES6(function(resolve) {
      if (!_this._model.collection.buffer) {
        process.nextTick(function() {
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>constructor (obj, options)](#apidoc.element.mongoose.schema.prototype.constructor)
- description and source-code
```javascript
function Schema(obj, options) {
  if (!(this instanceof Schema)) {
    return new Schema(obj, options);
  }

  this.obj = obj;
  this.paths = {};
  this.subpaths = {};
  this.virtuals = {};
  this.singleNestedPaths = {};
  this.nested = {};
  this.inherits = {};
  this.callQueue = [];
  this._indexes = [];
  this.methods = {};
  this.statics = {};
  this.tree = {};
  this.query = {};
  this.childSchemas = [];

  this.s = {
    hooks: new Kareem(),
    kareemHooks: IS_KAREEM_HOOK
  };

  this.options = this.defaultOptions(options);

  // build paths
  if (obj) {
    this.add(obj);
  }

  // check if _id's value is a subdocument (gh-2276)
  var _idSubDoc = obj && obj._id && utils.isObject(obj._id);

  // ensure the documents get an auto _id unless disabled
  var auto_id = !this.paths['_id'] &&
      (!this.options.noId && this.options._id) && !_idSubDoc;

  if (auto_id) {
    obj = {_id: {auto: true}};
    obj._id[this.options.typeKey] = Schema.ObjectId;
    this.add(obj);
  }

  // ensure the documents receive an id getter unless disabled
  var autoid = !this.paths['id'] &&
      (!this.options.noVirtualId && this.options.id);
  if (autoid) {
    this.virtual('id').get(idGetter);
  }

  for (var i = 0; i < this._defaultMiddleware.length; ++i) {
    var m = this._defaultMiddleware[i];
    this[m.kind](m.hook, !!m.isAsync, m.fn);
  }

  if (this.options.timestamps) {
    this.setupTimestamp(this.options.timestamps);
  }
}
```
- example usage
```shell
...
}

if (obj.constructor) {
  switch (exports.getFunctionName(obj.constructor)) {
    case 'Object':
      return cloneObject(obj, options);
    case 'Date':
      return new obj.constructor(+obj);
    case 'RegExp':
      return cloneRegExp(obj);
    default:
      // ignore
      break;
  }
}
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.defaultOptions"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>defaultOptions (options)](#apidoc.element.mongoose.schema.prototype.defaultOptions)
- description and source-code
```javascript
defaultOptions = function (options) {
  if (options && options.safe === false) {
    options.safe = {w: 0};
  }

  if (options && options.safe && options.safe.w === 0) {
    // if you turn off safe writes, then versioning goes off as well
    options.versionKey = false;
  }

  options = utils.options({
    strict: true,
    bufferCommands: true,
    capped: false, // { size, max, autoIndexId }
    versionKey: '__v',
    discriminatorKey: '__t',
    minimize: true,
    autoIndex: null,
    shardKey: null,
    read: null,
    validateBeforeSave: true,
    // the following are only applied at construction time
    noId: false, // deprecated, use { _id: false }
    _id: true,
    noVirtualId: false, // deprecated, use { id: false }
    id: true,
    typeKey: 'type',
    retainKeyOrder: false
  }, options);

  if (options.read) {
    options.read = readPref(options.read);
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.eachPath"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>eachPath (fn)](#apidoc.element.mongoose.schema.prototype.eachPath)
- description and source-code
```javascript
eachPath = function (fn) {
  var keys = Object.keys(this.paths),
      len = keys.length;

  for (var i = 0; i < len; ++i) {
    fn(keys[i], this.paths[keys[i]]);
  }

  return this;
}
```
- example usage
```shell
...
  var analyzeSchema = function(schema, prefix) {
    prefix || (prefix = '');

    // avoid recursion
    if (~seen.indexOf(schema)) return;
    seen.push(schema);

    schema.eachPath(function(path, type) {
if (prefix) path = prefix + '.' + path;

analyzePath(path, type);

// array of subdocs?
if (type.schema) {
  analyzeSchema(type.schema, path);
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.get"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>get (key)](#apidoc.element.mongoose.schema.prototype.get)
- description and source-code
```javascript
get = function (key) {
  return this.options[key];
}
```
- example usage
```shell
...
// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.hasMixedParent"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>hasMixedParent (path)](#apidoc.element.mongoose.schema.prototype.hasMixedParent)
- description and source-code
```javascript
hasMixedParent = function (path) {
  var subpaths = path.split(/\./g);
  path = '';
  for (var i = 0; i < subpaths.length; ++i) {
    path = i > 0 ? path + '.' + subpaths[i] : subpaths[i];
    if (path in this.paths &&
        this.paths[path] instanceof MongooseTypes.Mixed) {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.index"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>index (fields, options)](#apidoc.element.mongoose.schema.prototype.index)
- description and source-code
```javascript
index = function (fields, options) {
  options || (options = {});

  if (options.expires) {
    utils.expires(options);
  }

  this._indexes.push([fields, options]);
  return this;
}
```
- example usage
```shell
...
* ####Example:
*
*     var s = new Schema({ name: { type: String, index: true })
*     var s = new Schema({ loc: { type: [Number], index: 'hashed' })
*     var s = new Schema({ loc: { type: [Number], index: '2d', sparse: true })
*     var s = new Schema({ loc: { type: [Number], index: { type: '2dsphere', sparse: true }})
*     var s = new Schema({ date: { type: Date, index: { unique: true, expires: '1d' }})
*     Schema.path('my.path').index(true);
*     Schema.path('my.date').index({ expires: 60 });
*     Schema.path('my.path').index({ unique: true, sparse: true });
*
* ####NOTE:
*
* _Indexes are created in the background by default. Specify 'background: false' to override._
*
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.indexedPaths"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>indexedPaths ()](#apidoc.element.mongoose.schema.prototype.indexedPaths)
- description and source-code
```javascript
function indexedPaths() {
  if (this._indexedpaths) {
    return this._indexedpaths;
  }
  this._indexedpaths = this.indexes();
  return this._indexedpaths;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.indexes"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>indexes ()](#apidoc.element.mongoose.schema.prototype.indexes)
- description and source-code
```javascript
indexes = function () {
  'use strict';

  var indexes = [];
  var seenPrefix = {};

  var collectIndexes = function(schema, prefix) {
    if (seenPrefix[prefix]) {
      return;
    }
    seenPrefix[prefix] = true;

    prefix = prefix || '';
    var key, path, index, field, isObject, options, type;
    var keys = Object.keys(schema.paths);

    for (var i = 0; i < keys.length; ++i) {
      key = keys[i];
      path = schema.paths[key];

      if ((path instanceof MongooseTypes.DocumentArray) || path.$isSingleNested) {
        collectIndexes(path.schema, key + '.');
      } else {
        index = path._index;

        if (index !== false && index !== null && index !== undefined) {
          field = {};
          isObject = utils.isObject(index);
          options = isObject ? index : {};
          type = typeof index === 'string' ? index :
              isObject ? index.type :
                  false;

          if (type && ~Schema.indexTypes.indexOf(type)) {
            field[prefix + key] = type;
          } else if (options.text) {
            field[prefix + key] = 'text';
            delete options.text;
          } else {
            field[prefix + key] = 1;
          }

          delete options.type;
          if (!('background' in options)) {
            options.background = true;
          }

          indexes.push([field, options]);
        }
      }
    }

    if (prefix) {
      fixSubIndexPaths(schema, prefix);
    } else {
      schema._indexes.forEach(function(index) {
        if (!('background' in index[1])) {
          index[1].background = true;
        }
      });
      indexes = indexes.concat(schema._indexes);
    }
  };

  collectIndexes(this);
  return indexes;

<span class="apidocCodeCommentSpan">  /*!
   * Checks for indexes added to subdocs using Schema.index().
   * These indexes need their paths prefixed properly.
   *
   * schema._indexes = [ [indexObj, options], [indexObj, options] ..]
   */
</span>
  function fixSubIndexPaths(schema, prefix) {
    var subindexes = schema._indexes,
        len = subindexes.length,
        indexObj,
        newindex,
        klen,
        keys,
        key,
        i = 0,
        j;

    for (i = 0; i < len; ++i) {
      indexObj = subindexes[i][0];
      keys = Object.keys(indexObj);
      klen = keys.length;
      newindex = {};

      // use forward iteration, order matters
      for (j = 0; j < klen; ++j) {
        key = keys[j];
        newindex[prefix + key] = indexObj[key];
      }

      indexes.push([newindex, subindexes[i][1]]);
    }
  }
}
```
- example usage
```shell
...
    callback && callback();
    resolve();
  });
});
};

function _ensureIndexes(model, options, callback) {
var indexes = model.schema.indexes();
if (!indexes.length) {
  setImmediate(function() {
    callback && callback();
  });
  return;
}
// Indexes are created one-by-one to support how MongoDB < 2.4 deals
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.loadClass"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>loadClass (model, virtualsOnly)](#apidoc.element.mongoose.schema.prototype.loadClass)
- description and source-code
```javascript
loadClass = function (model, virtualsOnly) {
  if (model === Object.prototype ||
      model === Function.prototype ||
      model.prototype.hasOwnProperty('$isMongooseModelPrototype')) {
    return this;
  }

  // Add static methods
  if (!virtualsOnly) {
    Object.getOwnPropertyNames(model).forEach(function(name) {
      if (name.match(/^(length|name|prototype)$/)) {
        return;
      }
      var method = Object.getOwnPropertyDescriptor(model, name);
      if (typeof method.value === 'function') this.static(name, method.value);
    }, this);
  }

  // Add methods and virtuals
  Object.getOwnPropertyNames(model.prototype).forEach(function(name) {
    if (name.match(/^(constructor)$/)) {
      return;
    }
    var method = Object.getOwnPropertyDescriptor(model.prototype, name);
    if (!virtualsOnly) {
      if (typeof method.value === 'function') {
        this.method(name, method.value);
      }
    }
    if (typeof method.get === 'function') {
      this.virtual(name).get(method.get);
    }
    if (typeof method.set === 'function') {
      this.virtual(name).set(method.set);
    }
  }, this);

  return (this.loadClass(Object.getPrototypeOf(model)));
}
```
- example usage
```shell
...
  schema.add(o);
}

var model;
if (typeof name === 'function' && name.prototype instanceof Model) {
  model = name;
  name = model.name;
  schema.loadClass(model, true);
  model.prototype.$isMongooseModelPrototype = true;
} else {
  // generate new class
  model = function model(doc, fields, skipId) {
    if (!(this instanceof model)) {
      return new model(doc, fields, skipId);
    }
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.method"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>method (name, fn)](#apidoc.element.mongoose.schema.prototype.method)
- description and source-code
```javascript
method = function (name, fn) {
  if (typeof name !== 'string') {
    for (var i in name) {
      this.methods[i] = name[i];
    }
  } else {
    this.methods[name] = fn;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.path"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>path (path, obj)](#apidoc.element.mongoose.schema.prototype.path)
- description and source-code
```javascript
path = function (path, obj) {
  if (obj === undefined) {
    if (this.paths[path]) {
      return this.paths[path];
    }
    if (this.subpaths[path]) {
      return this.subpaths[path];
    }
    if (this.singleNestedPaths[path]) {
      return this.singleNestedPaths[path];
    }

    // subpaths?
    return /\.\d+\.?.*$/.test(path)
        ? getPositionalPath(this, path)
        : undefined;
  }

  // some path names conflict with document methods
  if (reserved[path]) {
    throw new Error(''' + path + '' may not be used as a schema pathname');
  }

  if (warnings[path]) {
    console.log('WARN: ' + warnings[path]);
  }

  // update the tree
  var subpaths = path.split(/\./),
      last = subpaths.pop(),
      branch = this.tree;

  subpaths.forEach(function(sub, i) {
    if (!branch[sub]) {
      branch[sub] = {};
    }
    if (typeof branch[sub] !== 'object') {
      var msg = 'Cannot set nested path '' + path + ''. '
          + 'Parent path ''
          + subpaths.slice(0, i).concat([sub]).join('.')
          + '' already set to type ' + branch[sub].name
          + '.';
      throw new Error(msg);
    }
    branch = branch[sub];
  });

  branch[last] = utils.clone(obj);

  this.paths[path] = Schema.interpretAsType(path, obj, this.options);

  if (this.paths[path].$isSingleNested) {
    for (var key in this.paths[path].schema.paths) {
      this.singleNestedPaths[path + '.' + key] =
          this.paths[path].schema.paths[key];
    }
    for (key in this.paths[path].schema.singleNestedPaths) {
      this.singleNestedPaths[path + '.' + key] =
          this.paths[path].schema.singleNestedPaths[key];
    }

    this.childSchemas.push(this.paths[path].schema);
  } else if (this.paths[path].$isMongooseDocumentArray) {
    this.childSchemas.push(this.paths[path].schema);
  }
  return this;
}
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.pathType"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>pathType (path)](#apidoc.element.mongoose.schema.prototype.pathType)
- description and source-code
```javascript
pathType = function (path) {
  if (path in this.paths) {
    return 'real';
  }
  if (path in this.virtuals) {
    return 'virtual';
  }
  if (path in this.nested) {
    return 'nested';
  }
  if (path in this.subpaths) {
    return 'real';
  }
  if (path in this.singleNestedPaths) {
    return 'real';
  }

  if (/\.\d+\.|\.\d+$/.test(path)) {
    return getPositionalPathType(this, path);
  }
  return 'adhocOrUndefined';
}
```
- example usage
```shell
...
  return this;
}
  }

  function _handleIndex(i) {
key = keys[i];
var pathName = prefix + key;
pathtype = this.schema.pathType(pathName);

if (path[key] !== null
    && path[key] !== void 0
      // need to know if plain object - no Buffer, ObjectId, ref, etc
    && utils.isObject(path[key])
    && (!path[key].constructor || utils.getFunctionName(path[key].constructor) === 'Object')
    && pathtype !== 'virtual'
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.plugin"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>plugin (fn, opts)](#apidoc.element.mongoose.schema.prototype.plugin)
- description and source-code
```javascript
plugin = function (fn, opts) {
  fn(this, opts);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.post"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>post (method, fn)](#apidoc.element.mongoose.schema.prototype.post)
- description and source-code
```javascript
post = function (method, fn) {
  if (IS_KAREEM_HOOK[method]) {
    this.s.hooks.post.apply(this.s.hooks, arguments);
    return this;
  }
  // assuming that all callbacks with arity < 2 are synchronous post hooks
  if (fn.length < 2) {
    return this.queue('on', [arguments[0], function(doc) {
      return fn.call(doc, doc);
    }]);
  }

  if (fn.length === 3) {
    this.s.hooks.post(method + ':error', fn);
    return this;
  }

  return this.queue('post', [arguments[0], function(next) {
    // wrap original function so that the callback goes last,
    // for compatibility with old code that is using synchronous post hooks
    var _this = this;
    var args = Array.prototype.slice.call(arguments, 1);
    fn.call(this, this, function(err) {
      return next.apply(_this, [err].concat(args));
    });
  }]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.pre"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>pre ()](#apidoc.element.mongoose.schema.prototype.pre)
- description and source-code
```javascript
pre = function () {
  var name = arguments[0];
  if (IS_KAREEM_HOOK[name]) {
    this.s.hooks.pre.apply(this.s.hooks, arguments);
    return this;
  }
  return this.queue('pre', arguments);
}
```
- example usage
```shell
...

// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.queue"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>queue (name, args)](#apidoc.element.mongoose.schema.prototype.queue)
- description and source-code
```javascript
queue = function (name, args) {
  this.callQueue.push([name, args]);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.remove"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>remove (path)](#apidoc.element.mongoose.schema.prototype.remove)
- description and source-code
```javascript
remove = function (path) {
  if (typeof path === 'string') {
    path = [path];
  }
  if (Array.isArray(path)) {
    path.forEach(function(name) {
      if (this.path(name)) {
        delete this.paths[name];

        var pieces = name.split('.');
        var last = pieces.pop();
        var branch = this.tree;
        for (var i = 0; i < pieces.length; ++i) {
          branch = branch[pieces[i]];
        }
        delete branch[last];
      }
    }, this);
  }
}
```
- example usage
```shell
...
'''

The same goes for removing them:

'''js
BlogPost.findById(myId, function (err, post) {
  if (!err) {
    post.comments[0].remove();
    post.save(function (err) {
      // do something
    });
  }
});
'''
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.requiredPaths"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>requiredPaths (invalidate)](#apidoc.element.mongoose.schema.prototype.requiredPaths)
- description and source-code
```javascript
function requiredPaths(invalidate) {
  if (this._requiredpaths && !invalidate) {
    return this._requiredpaths;
  }

  var paths = Object.keys(this.paths),
      i = paths.length,
      ret = [];

  while (i--) {
    var path = paths[i];
    if (this.paths[path].isRequired) {
      ret.push(path);
    }
  }
  this._requiredpaths = ret;
  return this._requiredpaths;
}
```
- example usage
```shell
...
  this.$__.strictMode = fields;
  fields = undefined;
} else {
  this.$__.strictMode = this.schema.options && this.schema.options.strict;
  this.$__.selected = fields;
}

var required = this.schema.requiredPaths();
for (var i = 0; i < required.length; ++i) {
  this.$__.activePaths.require(required[i]);
}

this.$__.emitter.setMaxListeners(0);
this._doc = this.$__buildDoc(obj, fields, skipId);
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.set"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>set (key, value, _tags)](#apidoc.element.mongoose.schema.prototype.set)
- description and source-code
```javascript
set = function (key, value, _tags) {
  if (arguments.length === 1) {
    return this.options[key];
  }

  switch (key) {
    case 'read':
      this.options[key] = readPref(value, _tags);
      break;
    case 'safe':
      this.options[key] = value === false
          ? {w: 0}
          : value;
      break;
    case 'timestamps':
      this.setupTimestamp(value);
      this.options[key] = value;
      break;
    default:
      this.options[key] = value;
  }

  return this;
}
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.setupTimestamp"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>setupTimestamp (timestamps)](#apidoc.element.mongoose.schema.prototype.setupTimestamp)
- description and source-code
```javascript
setupTimestamp = function (timestamps) {
  if (timestamps) {
    var createdAt = timestamps.createdAt || 'createdAt';
    var updatedAt = timestamps.updatedAt || 'updatedAt';
    var schemaAdditions = {};

    var parts = createdAt.split('.');
    var i;
    var cur = schemaAdditions;
    for (i = 0; i < parts.length; ++i) {
      cur[parts[i]] = (i < parts.length - 1 ?
        cur[parts[i]] || {} :
        Date);
    }

    parts = updatedAt.split('.');
    cur = schemaAdditions;
    for (i = 0; i < parts.length; ++i) {
      cur[parts[i]] = (i < parts.length - 1 ?
        cur[parts[i]] || {} :
        Date);
    }

    this.add(schemaAdditions);

    this.pre('save', function(next) {
      var defaultTimestamp = new Date();
      var auto_id = this._id && this._id.auto;

      if (!this.get(createdAt) && this.isSelected(createdAt)) {
        this.set(createdAt, auto_id ? this._id.getTimestamp() : defaultTimestamp);
      }

      if (this.isNew || this.isModified()) {
        this.set(updatedAt, this.isNew ? this.get(createdAt) : defaultTimestamp);
      }

      next();
    });

    var genUpdates = function(currentUpdate, overwrite) {
      var now = new Date();
      var updates = {};
      if (overwrite) {
        if (!currentUpdate[updatedAt]) {
          updates[updatedAt] = now;
        }
        if (!currentUpdate[createdAt]) {
          updates[createdAt] = now;
        }
        return updates;
      }
      updates = { $set: {}, $setOnInsert: {} };
      currentUpdate = currentUpdate || {};
      currentUpdate.$set = currentUpdate.$set || {};
      currentUpdate.$setOnInsert = currentUpdate.$setOnInsert || {};
      if (!currentUpdate[updatedAt] &&
          !currentUpdate.$set[updatedAt] &&
          !currentUpdate.$setOnInsert[updatedAt]) {
        updates.$set[updatedAt] = now;
      }
      if (!currentUpdate[createdAt] &&
          !currentUpdate.$set[createdAt] &&
          !currentUpdate.$setOnInsert[createdAt]) {
        updates.$setOnInsert[createdAt] = now;
      }

      return updates;
    };

    this.methods.initializeTimestamps = function() {
      if (!this.get(createdAt)) {
        this.set(createdAt, new Date());
      }
      if (!this.get(updatedAt)) {
        this.set(updatedAt, new Date());
      }
      return this;
    };

    this.pre('findOneAndUpdate', function(next) {
      var overwrite = this.options.overwrite;
      this.findOneAndUpdate({}, genUpdates(this.getUpdate(), overwrite), {
        overwrite: overwrite
      });
      applyTimestampsToChildren(this);
      next();
    });

    this.pre('update', function(next) {
      var overwrite = this.options.overwrite;
      this.update({}, genUpdates(this.getUpdate(), overwrite), {
        overwrite: overwrite
      });
      applyTimestampsToChildren(this);
      next();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.static"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>static (name, fn)](#apidoc.element.mongoose.schema.prototype.static)
- description and source-code
```javascript
static = function (name, fn) {
  if (typeof name !== 'string') {
    for (var i in name) {
      this.statics[i] = name[i];
    }
  } else {
    this.statics[name] = fn;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schema.prototype.virtual"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>virtual (name, options)](#apidoc.element.mongoose.schema.prototype.virtual)
- description and source-code
```javascript
virtual = function (name, options) {
  if (options && options.ref) {
    if (!options.localField) {
      throw new Error('Reference virtuals require 'localField' option');
    }

    if (!options.foreignField) {
      throw new Error('Reference virtuals require 'foreignField' option');
    }

    this.pre('init', function(next, obj) {
      if (name in obj) {
        if (!this.$$populatedVirtuals) {
          this.$$populatedVirtuals = {};
        }

        if (options.justOne) {
          this.$$populatedVirtuals[name] = Array.isArray(obj[name]) ?
            obj[name][0] :
            obj[name];
        } else {
          this.$$populatedVirtuals[name] = Array.isArray(obj[name]) ?
            obj[name] :
            obj[name] == null ? [] : [obj[name]];
        }

        delete obj[name];
      }
      if (this.ownerDocument) {
        next();
        return this;
      } else {
        next();
      }
    });

    var virtual = this.virtual(name);
    virtual.options = options;
    return virtual.
      get(function() {
        if (!this.$$populatedVirtuals) {
          this.$$populatedVirtuals = {};
        }
        if (name in this.$$populatedVirtuals) {
          return this.$$populatedVirtuals[name];
        }
        return null;
      }).
      set(function(v) {
        if (!this.$$populatedVirtuals) {
          this.$$populatedVirtuals = {};
        }
        this.$$populatedVirtuals[name] = v;
      });
  }

  var virtuals = this.virtuals;
  var parts = name.split('.');

  if (this.pathType(name) === 'real') {
    throw new Error('Virtual path "' + name + '"' +
      ' conflicts with a real path in the schema');
  }

  virtuals[name] = parts.reduce(function(mem, part, i) {
    mem[part] || (mem[part] = (i === parts.length - 1)
        ? new VirtualType(options, name)
        : {});
    return mem[part];
  }, this.tree);

  return virtuals[name];
}
```
- example usage
```shell
...
/**
 * VirtualType constructor
 *
 * This is what mongoose uses to define virtual attributes via 'Schema.prototype.virtual'.
 *
 * ####Example:
 *
 *     var fullname = schema.virtual('fullname');
 *     fullname instanceof mongoose.VirtualType // true
 *
 * @parma {Object} options
 * @api public
 */

function VirtualType(options, name) {
...
```

#### <a name="apidoc.element.mongoose.schema.prototype.virtualpath"></a>[function <span class="apidocSignatureSpan">mongoose.schema.prototype.</span>virtualpath (name)](#apidoc.element.mongoose.schema.prototype.virtualpath)
- description and source-code
```javascript
virtualpath = function (name) {
  return this.virtuals[name];
}
```
- example usage
```shell
...
  if (!mixed) {
    if (strict === 'throw') {
      throw new StrictModeError(path);
    }
    return this;
  }
} else if (pathType === 'virtual') {
  schema = this.schema.virtualpath(path);
  schema.applySetters(val, this);
  return this;
} else {
  schema = this.$__path(path);
}

var pathToMark;
...
```



# <a name="apidoc.module.mongoose.schematype"></a>[module mongoose.schematype](#apidoc.module.mongoose.schematype)

#### <a name="apidoc.element.mongoose.schematype.schematype"></a>[function <span class="apidocSignatureSpan">mongoose.</span>schematype (path, options, instance)](#apidoc.element.mongoose.schematype.schematype)
- description and source-code
```javascript
function SchemaType(path, options, instance) {
  this.path = path;
  this.instance = instance;
  this.validators = [];
  this.setters = [];
  this.getters = [];
  this.options = options;
  this._index = null;
  this.selected;

  for (var i in options) {
    if (this[i] && typeof this[i] === 'function') {
      // { unique: true, index: true }
      if (i === 'index' && this._index) {
        continue;
      }

      var opts = Array.isArray(options[i])
          ? options[i]
          : [options[i]];

      this[i].apply(this, opts);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schematype.CastError"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.</span>CastError (type, value, path, reason)](#apidoc.element.mongoose.schematype.CastError)
- description and source-code
```javascript
function CastError(type, value, path, reason) {
  var stringValue = util.inspect(value);
  stringValue = stringValue.replace(/^'/, '"').replace(/'$/, '"');
  if (stringValue.charAt(0) !== '"') {
    stringValue = '"' + stringValue + '"';
  }
  MongooseError.call(this, 'Cast to ' + type + ' failed for value ' +
    stringValue + ' at path "' + path + '"');
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.stringValue = stringValue;
  this.name = 'CastError';
  this.kind = type;
  this.value = value;
  this.path = path;
  this.reason = reason;
}
```
- example usage
```shell
...
      this.markModified(path);
      cleanModifiedSubpaths(this, path);
    } else {
      this.set(val, path, constructing);
    }
    return this;
  }
  this.invalidate(path, new MongooseError.CastError('Object', val, path));
  return this;
}

var schema;
var parts = path.split('.');

if (pathType === 'adhocOrUndefined' && strict) {
...
```

#### <a name="apidoc.element.mongoose.schematype.ValidatorError"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.</span>ValidatorError (properties)](#apidoc.element.mongoose.schematype.ValidatorError)
- description and source-code
```javascript
function ValidatorError(properties) {
  var msg = properties.message;
  if (!msg) {
    msg = MongooseError.messages.general.default;
  }

  var message = this.formatMessage(msg, properties);
  MongooseError.call(this, message);
  if (Error.captureStackTrace) {
    Error.captureStackTrace(this);
  } else {
    this.stack = new Error().stack;
  }
  this.properties = properties;
  this.name = 'ValidatorError';
  this.kind = properties.type;
  this.path = properties.path;
  this.value = properties.value;
  this.reason = properties.reason;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schematype._isRef"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.</span>_isRef (self, value, doc, init)](#apidoc.element.mongoose.schematype._isRef)
- description and source-code
```javascript
_isRef = function (self, value, doc, init) {
  // fast path
  var ref = init && self.options && self.options.ref;

  if (!ref && doc && doc.$__fullPath) {
    // checks for
    // - this populated with adhoc model and no ref was set in schema OR
    // - setting / pushing values after population
    var path = doc.$__fullPath(self.path);
    var owner = doc.ownerDocument ? doc.ownerDocument() : doc;
    ref = owner.populated(path);
  }

  if (ref) {
    if (value == null) {
      return true;
    }
    if (!Buffer.isBuffer(value) &&  // buffers are objects too
        value._bsontype !== 'Binary' // raw binary value from the db
        && utils.isObject(value)    // might have deselected _id in population query
    ) {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.schematype.prototype"></a>[module mongoose.schematype.prototype](#apidoc.module.mongoose.schematype.prototype)

#### <a name="apidoc.element.mongoose.schematype.prototype.applyGetters"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>applyGetters (value, scope)](#apidoc.element.mongoose.schematype.prototype.applyGetters)
- description and source-code
```javascript
applyGetters = function (value, scope) {
  var v = value,
      getters = this.getters,
      len = getters.length;

  if (!len) {
    return v;
  }

  while (len--) {
    v = getters[len].call(scope, v, this);
  }

  return v;
}
```
- example usage
```shell
...
 if (adhoc) {
   obj = adhoc.cast(obj);
 }

 // Check if this path is populated - don't apply getters if it is,
 // because otherwise its a nested object. See gh-3357
 if (schema && !this.populated(path)) {
   obj = schema.applyGetters(obj, this);
 }

 return obj;
};

/**
* Returns the schematype for the given 'path'.
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.applySetters"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>applySetters (value, scope, init, priorVal, options)](#apidoc.element.mongoose.schematype.prototype.applySetters)
- description and source-code
```javascript
applySetters = function (value, scope, init, priorVal, options) {
  var v = value,
      setters = this.setters,
      len = setters.length,
      caster = this.caster;

  while (len--) {
    v = setters[len].call(scope, v, this);
  }

  if (Array.isArray(v) && caster && caster.setters) {
    var newVal = [];
    for (var i = 0; i < v.length; i++) {
      newVal.push(caster.applySetters(v[i], scope, init, priorVal));
    }
    v = newVal;
  }

  if (v === null || v === undefined) {
    return v;
  }

  // do not cast until all setters are applied #665
  v = this.cast(v, scope, init, priorVal, options);

  return v;
}
```
- example usage
```shell
...
    if (strict === 'throw') {
      throw new StrictModeError(path);
    }
    return this;
  }
} else if (pathType === 'virtual') {
  schema = this.schema.virtualpath(path);
  schema.applySetters(val, this);
  return this;
} else {
  schema = this.$__path(path);
}

var pathToMark;
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.castForQuery"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>castForQuery ($conditional, val)](#apidoc.element.mongoose.schematype.prototype.castForQuery)
- description and source-code
```javascript
castForQuery = function ($conditional, val) {
  var handler;
  if (arguments.length === 2) {
    handler = this.$conditionalHandlers[$conditional];
    if (!handler) {
      throw new Error('Can\'t use ' + $conditional);
    }
    return handler.call(this, val);
  }
  val = $conditional;
  return this.cast(val);
}
```
- example usage
```shell
...
          }

          if (geo) {
var numbertype = new Types.Number('__QueryCasting__');
var value = val[geo];

if (val.$maxDistance != null) {
  val.$maxDistance = numbertype.castForQuery(val.$maxDistance);
}
if (val.$minDistance != null) {
  val.$minDistance = numbertype.castForQuery(val.$minDistance);
}

if (geo === '$within') {
  var withinType = value.$center
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.checkRequired"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>checkRequired (val)](#apidoc.element.mongoose.schematype.prototype.checkRequired)
- description and source-code
```javascript
checkRequired = function (val) {
  return val != null;
}
```
- example usage
```shell
...
  // in here, 'this' refers to the validating document.
  // no validation when this path wasn't selected in the query.
  if ('isSelected' in this && !this.isSelected(_this.path) && !this.isModified(_this.path)) {
    return true;
  }

  return ((typeof required === 'function') && !required.apply(this)) ||
      _this.checkRequired(v, this);
};
this.originalRequiredValue = required;

if (typeof required === 'string') {
  message = required;
  required = undefined;
}
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.default"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>default (val)](#apidoc.element.mongoose.schematype.prototype.default)
- description and source-code
```javascript
default = function (val) {
  if (arguments.length === 1) {
    if (val === void 0) {
      this.defaultValue = void 0;
      return void 0;
    }
    this.defaultValue = val;
    return this.defaultValue;
  } else if (arguments.length > 1) {
    this.defaultValue = utils.args(arguments);
  }
  return this.defaultValue;
}
```
- example usage
```shell
...
  if (p in fields) {
    continue;
  }

  def = type.getDefault(_this, false);
  if (typeof def !== 'undefined') {
    doc_[piece] = def;
    _this.$__.activePaths.default(p);
  }
} else if (included) {
  // selected field
  def = type.getDefault(_this, false);
  if (typeof def !== 'undefined') {
    doc_[piece] = def;
    _this.$__.activePaths.default(p);
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.doValidate"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>doValidate (value, fn, scope)](#apidoc.element.mongoose.schematype.prototype.doValidate)
- description and source-code
```javascript
doValidate = function (value, fn, scope) {
  var err = false;
  var path = this.path;
  var count = this.validators.length;

  if (!count) {
    return fn(null);
  }

  var validate = function(ok, validatorProperties) {
    if (err) {
      return;
    }
    if (ok === undefined || ok) {
      --count || fn(null);
    } else {
      err = new ValidatorError(validatorProperties);
      fn(err);
    }
  };

  var _this = this;
  this.validators.forEach(function(v) {
    if (err) {
      return;
    }

    var validator = v.validator;
    var ok;

    var validatorProperties = utils.clone(v);
    validatorProperties.path = path;
    validatorProperties.value = value;

    if (validator instanceof RegExp) {
      validate(validator.test(value), validatorProperties);
    } else if (typeof validator === 'function') {
      if (value === undefined && !_this.isRequired) {
        validate(true, validatorProperties);
        return;
      }
      if (validatorProperties.isAsync) {
        asyncValidate(validator, scope, value, validatorProperties, validate);
      } else if (validator.length === 2 && !('isAsync' in validatorProperties)) {
        legacyAsyncValidate(validator, scope, value, validatorProperties,
          validate);
      } else {
        try {
          ok = validator.call(scope, value);
        } catch (error) {
          ok = false;
          validatorProperties.reason = error;
        }
        if (ok && typeof ok.then === 'function') {
          ok.then(
            function(ok) { validate(ok, validatorProperties); },
            function(error) {
              validatorProperties.reason = error;
              ok = false;
              validate(ok, validatorProperties);
            });
        } else {
          validate(ok, validatorProperties);
        }
      }
    }
  });
}
```
- example usage
```shell
...
    // If user marked as invalid or there was a cast error, don't validate
    if (!_this.$isValid(path)) {
      --total || complete();
      return;
    }

    var val = _this.getValue(path);
    p.doValidate(val, function(err) {
      if (err) {
        _this.invalidate(path, err, undefined, true);
      }
      --total || complete();
    }, _this);
  });
};
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.doValidateSync"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>doValidateSync (value, scope)](#apidoc.element.mongoose.schematype.prototype.doValidateSync)
- description and source-code
```javascript
doValidateSync = function (value, scope) {
  var err = null,
      path = this.path,
      count = this.validators.length;

  if (!count) {
    return null;
  }

  var validate = function(ok, validatorProperties) {
    if (err) {
      return;
    }
    if (ok !== undefined && !ok) {
      err = new ValidatorError(validatorProperties);
    }
  };

  var validators = this.validators;
  if (value === void 0) {
    if (this.validators.length > 0 && this.validators[0].type === 'required') {
      validators = [this.validators[0]];
    } else {
      return null;
    }
  }

  validators.forEach(function(v) {
    if (err) {
      return;
    }

    var validator = v.validator;
    var validatorProperties = utils.clone(v);
    validatorProperties.path = path;
    validatorProperties.value = value;
    var ok;

    if (validator instanceof RegExp) {
      validate(validator.test(value), validatorProperties);
    } else if (typeof validator === 'function') {
      // if not async validators
      if (validator.length !== 2 && !validatorProperties.isAsync) {
        try {
          ok = validator.call(scope, value);
        } catch (error) {
          ok = false;
          validatorProperties.reason = error;
        }
        validate(ok, validatorProperties);
      }
    }
  });

  return err;
}
```
- example usage
```shell
...
    return;
  }
  if (!_this.$isValid(path)) {
    return;
  }

  var val = _this.getValue(path);
  var err = p.doValidateSync(val, _this);
  if (err) {
    _this.invalidate(path, err, undefined, true);
  }
});

var err = _this.$__.validationError;
_this.$__.validationError = undefined;
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.get"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>get (fn)](#apidoc.element.mongoose.schematype.prototype.get)
- description and source-code
```javascript
get = function (fn) {
  if (typeof fn !== 'function') {
    throw new TypeError('A getter must be a function.');
  }
  this.getters.push(fn);
  return this;
}
```
- example usage
```shell
...
// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.getDefault"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>getDefault (scope, init)](#apidoc.element.mongoose.schematype.prototype.getDefault)
- description and source-code
```javascript
getDefault = function (scope, init) {
  var ret = typeof this.defaultValue === 'function'
      ? this.defaultValue.call(scope)
      : this.defaultValue;

  if (ret !== null && ret !== undefined) {
    var casted = this.cast(ret, scope, init);
    if (casted && casted.$isSingleNested) {
      casted.$parent = scope;
    }
    return casted;
  }
  return ret;
}
```
- example usage
```shell
...
        if (fields && exclude !== null) {
if (exclude === true) {
  // apply defaults to all non-excluded fields
  if (p in fields) {
    continue;
  }

  def = type.getDefault(_this, false);
  if (typeof def !== 'undefined') {
    doc_[piece] = def;
    _this.$__.activePaths.default(p);
  }
} else if (included) {
  // selected field
  def = type.getDefault(_this, false);
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.index"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>index (options)](#apidoc.element.mongoose.schematype.prototype.index)
- description and source-code
```javascript
index = function (options) {
  this._index = options;
  utils.expires(this._index);
  return this;
}
```
- example usage
```shell
...
* ####Example:
*
*     var s = new Schema({ name: { type: String, index: true })
*     var s = new Schema({ loc: { type: [Number], index: 'hashed' })
*     var s = new Schema({ loc: { type: [Number], index: '2d', sparse: true })
*     var s = new Schema({ loc: { type: [Number], index: { type: '2dsphere', sparse: true }})
*     var s = new Schema({ date: { type: Date, index: { unique: true, expires: '1d' }})
*     Schema.path('my.path').index(true);
*     Schema.path('my.date').index({ expires: 60 });
*     Schema.path('my.path').index({ unique: true, sparse: true });
*
* ####NOTE:
*
* _Indexes are created in the background by default. Specify 'background: false' to override._
*
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.required"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>required (required, message)](#apidoc.element.mongoose.schematype.prototype.required)
- description and source-code
```javascript
required = function (required, message) {
  if (required === false) {
    this.validators = this.validators.filter(function(v) {
      return v.validator !== this.requiredValidator;
    }, this);

    this.isRequired = false;
    return this;
  }

  var _this = this;
  this.isRequired = true;

  this.requiredValidator = function(v) {
    // in here, 'this' refers to the validating document.
    // no validation when this path wasn't selected in the query.
    if ('isSelected' in this && !this.isSelected(_this.path) && !this.isModified(_this.path)) {
      return true;
    }

    return ((typeof required === 'function') && !required.apply(this)) ||
        _this.checkRequired(v, this);
  };
  this.originalRequiredValue = required;

  if (typeof required === 'string') {
    message = required;
    required = undefined;
  }

  var msg = message || MongooseError.messages.general.required;
  this.validators.unshift({
    validator: this.requiredValidator,
    message: msg,
    type: 'required'
  });

  return this;
}
```
- example usage
```shell
...
*
*     // or with custom error message
*
*     var s = new Schema({ born: { type: Date, required: '{PATH} is required!' })
*
*     // or through the path API
*
*     Schema.path('name').required(true);
*
*     // with custom error messaging
*
*     Schema.path('name').required(true, 'grrr :( ');
*
*     // or make a path conditionally required based on a function
*     var isOver18 = function() { return this.age >= 18; };
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.select"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>select (val)](#apidoc.element.mongoose.schematype.prototype.select)
- description and source-code
```javascript
function select(val) {
  this.selected = !!val;
  return this;
}
```
- example usage
```shell
...
};

/**
* Checks if 'path' was selected in the source query which initialized this document.
*
* ####Example
*
*     Thing.findOne().select('name').exec(function (err, doc) {
*        doc.isSelected('name') // true
*        doc.isSelected('age')  // false
*     })
*
* @param {String} path
* @return {Boolean}
* @api public
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.set"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>set (fn)](#apidoc.element.mongoose.schematype.prototype.set)
- description and source-code
```javascript
set = function (fn) {
  if (typeof fn !== 'function') {
    throw new TypeError('A setter must be a function.');
  }
  this.setters.push(fn);
  return this;
}
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.sparse"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>sparse (bool)](#apidoc.element.mongoose.schematype.prototype.sparse)
- description and source-code
```javascript
sparse = function (bool) {
  if (this._index === null || this._index === undefined ||
    typeof this._index === 'boolean') {
    this._index = {};
  } else if (typeof this._index === 'string') {
    this._index = {type: this._index};
  }

  this._index.sparse = bool;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schematype.prototype.text"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>text (bool)](#apidoc.element.mongoose.schematype.prototype.text)
- description and source-code
```javascript
text = function (bool) {
  if (this._index === null || this._index === undefined ||
    typeof this._index === 'boolean') {
    this._index = {};
  } else if (typeof this._index === 'string') {
    this._index = {type: this._index};
  }

  this._index.text = bool;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.schematype.prototype.unique"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>unique (bool)](#apidoc.element.mongoose.schematype.prototype.unique)
- description and source-code
```javascript
unique = function (bool) {
  if (this._index === false) {
    if (!bool) {
      return;
    }
    throw new Error('Path "' + this.path + '" may not have 'index' set to ' +
      'false and 'unique' set to true');
  }
  if (this._index == null || this._index === true) {
    this._index = {};
  } else if (typeof this._index === 'string') {
    this._index = {type: this._index};
  }

  this._index.unique = bool;
  return this;
}
```
- example usage
```shell
...
if (mod.options.match) {
  match = utils.object.shallowCopy(mod.options.match);
} else {
  match = {};
}

var ids = utils.array.flatten(mod.ids, flatten);
ids = utils.array.unique(ids);

if (ids.length === 0 || ids.every(utils.isNullOrUndefined)) {
  --_remaining;
  continue;
}

hasOne = true;
...
```

#### <a name="apidoc.element.mongoose.schematype.prototype.validate"></a>[function <span class="apidocSignatureSpan">mongoose.schematype.prototype.</span>validate (obj, message, type)](#apidoc.element.mongoose.schematype.prototype.validate)
- description and source-code
```javascript
validate = function (obj, message, type) {
  if (typeof obj === 'function' || obj && utils.getFunctionName(obj.constructor) === 'RegExp') {
    var properties;
    if (message instanceof Object && !type) {
      properties = utils.clone(message);
      if (!properties.message) {
        properties.message = properties.msg;
      }
      properties.validator = obj;
      properties.type = properties.type || 'user defined';
    } else {
      if (!message) {
        message = MongooseError.messages.general.default;
      }
      if (!type) {
        type = 'user defined';
      }
      properties = {message: message, type: type, validator: obj};
    }
    this.validators.push(properties);
    return this;
  }

  var i,
      length,
      arg;

  for (i = 0, length = arguments.length; i < length; i++) {
    arg = arguments[i];
    if (!(arg && utils.getFunctionName(arg.constructor) === 'Object')) {
      var msg = 'Invalid validator. Received (' + typeof arg + ') '
          + arg
          + '. See http://mongoosejs.com/docs/api.html#schematype_SchemaType-validate';

      throw new Error(msg);
    }
    this.validate(arg.validator, arg);
  }

  return this;
}
```
- example usage
```shell
...
*
* ####Note:
*
* This method is called 'pre' save and if a validation rule is violated, [save](#model_Model-save) is aborted and the error is returned
 to your 'callback'.
*
* ####Example:
*
*     doc.validate(function (err) {
*       if (err) handleError(err);
*       else // validation passed
*     });
*
* @param {Object} optional options internal options
* @param {Function} callback optional callback called after validation completes, passing an error if one occurred
* @return {Promise} Promise
...
```



# <a name="apidoc.module.mongoose.statemachine"></a>[module mongoose.statemachine](#apidoc.module.mongoose.statemachine)

#### <a name="apidoc.element.mongoose.statemachine.statemachine"></a>[function <span class="apidocSignatureSpan">mongoose.</span>statemachine ()](#apidoc.element.mongoose.statemachine.statemachine)
- description and source-code
```javascript
function StateMachine() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.statemachine.ctor"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.</span>ctor ()](#apidoc.element.mongoose.statemachine.ctor)
- description and source-code
```javascript
ctor = function () {
  var states = utils.args(arguments);

  var ctor = function() {
    StateMachine.apply(this, arguments);
    this.paths = {};
    this.states = {};
    this.stateNames = states;

    var i = states.length,
        state;

    while (i--) {
      state = states[i];
      this.states[state] = {};
    }
  };

  ctor.prototype = new StateMachine();

  states.forEach(function(state) {
    // Changes the 'path''s state to 'state'.
    ctor.prototype[state] = function(path) {
      this._changeState(path, state);
    };
  });

  return ctor;
}
```
- example usage
```shell
...


/*!
 * Dependencies
 */

var StateMachine = require('./statemachine');
var ActiveRoster = StateMachine.ctor('require', 'modify', 'init', 'default', 'ignore');

module.exports = exports = InternalCache;

function InternalCache() {
this.strictMode = undefined;
this.selected = undefined;
this.shardval = undefined;
...
```



# <a name="apidoc.module.mongoose.statemachine.prototype"></a>[module mongoose.statemachine.prototype](#apidoc.module.mongoose.statemachine.prototype)

#### <a name="apidoc.element.mongoose.statemachine.prototype._changeState"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>_changeState (path, nextState)](#apidoc.element.mongoose.statemachine.prototype._changeState)
- description and source-code
```javascript
function _changeState(path, nextState) {
  var prevBucket = this.states[this.paths[path]];
  if (prevBucket) delete prevBucket[path];

  this.paths[path] = nextState;
  this.states[nextState][path] = true;
}
```
- example usage
```shell
...
  };

  ctor.prototype = new StateMachine();

  states.forEach(function(state) {
    // Changes the 'path''s state to 'state'.
    ctor.prototype[state] = function(path) {
      this._changeState(path, state);
    };
  });

  return ctor;
};

/*!
...
```

#### <a name="apidoc.element.mongoose.statemachine.prototype._iter"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>_iter (iterMethod)](#apidoc.element.mongoose.statemachine.prototype._iter)
- description and source-code
```javascript
function _iter(iterMethod) {
  return function() {
    var numArgs = arguments.length,
        states = utils.args(arguments, 0, numArgs - 1),
        callback = arguments[numArgs - 1];

    if (!states.length) states = this.stateNames;

    var _this = this;

    var paths = states.reduce(function(paths, state) {
      return paths.concat(Object.keys(_this.states[state]));
    }, []);

    return paths[iterMethod](function(path, i, paths) {
      return callback(path, i, paths);
    });
  };
}
```
- example usage
```shell
...
* @param {String} [state]
* @param {String} [state]
* @param {Function} callback
* @private
*/

StateMachine.prototype.forEach = function forEach() {
 this.forEach = this._iter('forEach');
 return this.forEach.apply(this, arguments);
};

/*!
* Maps over the paths that belong to one of the parameter states.
*
* The function profile can look like:
...
```

#### <a name="apidoc.element.mongoose.statemachine.prototype.clear"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>clear (state)](#apidoc.element.mongoose.statemachine.prototype.clear)
- description and source-code
```javascript
function clear(state) {
  var keys = Object.keys(this.states[state]),
      i = keys.length,
      path;

  while (i--) {
    path = keys[i];
    delete this.states[state][path];
    delete this.paths[path];
  }
}
```
- example usage
```shell
...
  var type = dirt.value;
  if (type && type._atomics) {
    type._atomics = {};
  }
});

// Clear 'dirty' cache
this.$__.activePaths.clear('modify');
this.$__.activePaths.clear('default');
this.$__.validationError = undefined;
this.errors = undefined;
_this = this;
this.schema.requiredPaths().forEach(function(path) {
  _this.$__.activePaths.require(path);
});
...
```

#### <a name="apidoc.element.mongoose.statemachine.prototype.forEach"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>forEach ()](#apidoc.element.mongoose.statemachine.prototype.forEach)
- description and source-code
```javascript
function forEach() {
  this.forEach = this._iter('forEach');
  return this.forEach.apply(this, arguments);
}
```
- example usage
```shell
...
 * @api public
 */

Aggregate.prototype.project = function(arg) {
var fields = {};

if (typeof arg === 'object' && !util.isArray(arg)) {
  Object.keys(arg).forEach(function(field) {
    fields[field] = arg[field];
  });
} else if (arguments.length === 1 && typeof arg === 'string') {
  arg.split(/\s+/).forEach(function(field) {
    if (!field) {
      return;
    }
...
```

#### <a name="apidoc.element.mongoose.statemachine.prototype.map"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>map ()](#apidoc.element.mongoose.statemachine.prototype.map)
- description and source-code
```javascript
function map() {
  this.map = this._iter('map');
  return this.map.apply(this, arguments);
}
```
- example usage
```shell
...
    val.length > 0 &&
    val[0] instanceof Document &&
    val[0].constructor.modelName &&
    (schema.options.type[0].ref === val[0].constructor.baseModelName || schema.options.type[0].ref === val[0].constructor.modelName
)) {
  if (this.ownerDocument) {
    popOpts = { model: val[0].constructor };
    this.ownerDocument().populated(this.$__fullPath(path),
      val.map(function(v) { return v._id; }), popOpts);
  } else {
    popOpts = { model: val[0].constructor };
    this.populated(path, val.map(function(v) { return v._id; }), popOpts);
  }
  didPopulate = true;
}
val = schema.applySetters(val, this, false, priorVal);
...
```

#### <a name="apidoc.element.mongoose.statemachine.prototype.some"></a>[function <span class="apidocSignatureSpan">mongoose.statemachine.prototype.</span>some ()](#apidoc.element.mongoose.statemachine.prototype.some)
- description and source-code
```javascript
function some() {
  var _this = this;
  var what = arguments.length ? arguments : this.stateNames;
  return Array.prototype.some.call(what, function(state) {
    return Object.keys(_this.states[state]).length;
  });
}
```
- example usage
```shell
...
 if (typeof obj !== 'object') {
   return false;
 }

 k = Object.keys(obj);

 return k.length === 1 && k
         .some(function(key) {
           return key[0] === '$';
         });
}

/*!
* Adds the appropriate '$match' pipeline step to the top of an aggregate's
* pipeline, should it's model is a non-root discriminator type. This is
...
```



# <a name="apidoc.module.mongoose.types"></a>[module mongoose.types](#apidoc.module.mongoose.types)

#### <a name="apidoc.element.mongoose.types.Array"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Array (values, path, doc)](#apidoc.element.mongoose.types.Array)
- description and source-code
```javascript
function MongooseArray(values, path, doc) {
  var arr = [].concat(values);

  var keysMA = Object.keys(MongooseArray.mixin);
  var numKeys = keysMA.length;
  for (var i = 0; i < numKeys; ++i) {
    arr[keysMA[i]] = MongooseArray.mixin[keysMA[i]];
  }

  arr._path = path;
  arr.isMongooseArray = true;
  arr.validators = [];
  arr._atomics = {};
  arr._schema = void 0;

  // Because doc comes from the context of another function, doc === global
  // can happen if there was a null somewhere up the chain (see #3020)
  // RB Jun 17, 2015 updated to check for presence of expected paths instead
  // to make more proof against unusual node environments
  if (doc && doc instanceof Document) {
    arr._parent = doc;
    arr._schema = doc.schema.path(path);
  }

  return arr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.Buffer"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Buffer (value, encode, offset)](#apidoc.element.mongoose.types.Buffer)
- description and source-code
```javascript
function MongooseBuffer(value, encode, offset) {
  var length = arguments.length;
  var val;

  if (length === 0 || arguments[0] === null || arguments[0] === undefined) {
    val = 0;
  } else {
    val = value;
  }

  var encoding;
  var path;
  var doc;

  if (Array.isArray(encode)) {
    // internal casting
    path = encode[0];
    doc = encode[1];
  } else {
    encoding = encode;
  }

  var buf = new Buffer(val, encoding, offset);
  utils.decorate(buf, MongooseBuffer.mixin);
  buf.isMongooseBuffer = true;

  // make sure these internal props don't show up in Object.keys()
  Object.defineProperties(buf, {
    validators: {value: []},
    _path: {value: path},
    _parent: {value: doc}
  });

  if (doc && typeof path === 'string') {
    Object.defineProperty(buf, '_schema', {
      value: doc.schema.path(path)
    });
  }

  buf._subtype = 0;
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.Decimal128"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Decimal128 (bytes)](#apidoc.element.mongoose.types.Decimal128)
- description and source-code
```javascript
Decimal128 = function (bytes) {
  this._bsontype = 'Decimal128';
  this.bytes = bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.Document"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Document (obj, parentArr, skipId, fields, index)](#apidoc.element.mongoose.types.Document)
- description and source-code
```javascript
function EmbeddedDocument(obj, parentArr, skipId, fields, index) {
  if (parentArr) {
    this.__parentArray = parentArr;
    this.__parent = parentArr._parent;
  } else {
    this.__parentArray = undefined;
    this.__parent = undefined;
  }
  this.__index = index;

  Document.call(this, obj, fields, skipId);

  var _this = this;
  this.on('isNew', function(val) {
    _this.isNew = val;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.DocumentArray"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>DocumentArray (values, path, doc)](#apidoc.element.mongoose.types.DocumentArray)
- description and source-code
```javascript
function MongooseDocumentArray(values, path, doc) {
  var arr = [].concat(values);
  arr._path = path;

  var props = {
    isMongooseArray: true,
    isMongooseDocumentArray: true,
    validators: [],
    _atomics: {},
    _schema: void 0,
    _handlers: void 0
  };

  // Values always have to be passed to the constructor to initialize, since
  // otherwise MongooseArray#push will mark the array as modified to the parent.
  var keysMA = Object.keys(MongooseArray.mixin);
  var numKeys = keysMA.length;
  for (var j = 0; j < numKeys; ++j) {
    arr[keysMA[j]] = MongooseArray.mixin[keysMA[j]];
  }

  var keysMDA = Object.keys(MongooseDocumentArray.mixin);
  numKeys = keysMDA.length;
  for (var i = 0; i < numKeys; ++i) {
    arr[keysMDA[i]] = MongooseDocumentArray.mixin[keysMDA[i]];
  }

  var keysP = Object.keys(props);
  numKeys = keysP.length;
  for (var k = 0; k < numKeys; ++k) {
    arr[keysP[k]] = props[keysP[k]];
  }

  // Because doc comes from the context of another function, doc === global
  // can happen if there was a null somewhere up the chain (see #3020 && #3034)
  // RB Jun 17, 2015 updated to check for presence of expected paths instead
  // to make more proof against unusual node environments
  if (doc && doc instanceof Document) {
    arr._parent = doc;
    arr._schema = doc.schema.path(path);
    arr._handlers = {
      isNew: arr.notify('isNew'),
      save: arr.notify('save')
    };

    doc.on('save', arr._handlers.save);
    doc.on('isNew', arr._handlers.isNew);
  }

  return arr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.Embedded"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Embedded (obj, parentArr, skipId, fields, index)](#apidoc.element.mongoose.types.Embedded)
- description and source-code
```javascript
function EmbeddedDocument(obj, parentArr, skipId, fields, index) {
  if (parentArr) {
    this.__parentArray = parentArr;
    this.__parent = parentArr._parent;
  } else {
    this.__parentArray = undefined;
    this.__parent = undefined;
  }
  this.__index = index;

  Document.call(this, obj, fields, skipId);

  var _this = this;
  this.on('isNew', function(val) {
    _this.isNew = val;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.types.ObjectId"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>ObjectId (id)](#apidoc.element.mongoose.types.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
...
*     .unwind('tags')
*     .exec(callback)
*
* ####Note:
*
* - The documents returned are plain javascript objects, not mongoose documents (since any shape of document can be returned).
* - Requires MongoDB >= 2.1
* - Mongoose does **not** cast pipeline stages. 'new Aggregate({ $match: { _id: '00000000000000000000000a' } });' will not work
unless '_id' is a string in the database. Use 'new Aggregate({ $match: { _id: mongoose.Types.ObjectId('00000000000000000000000a') } });'
instead.
*
* @see MongoDB http://docs.mongodb.org/manual/applications/aggregation/
* @see driver http://mongodb.github.com/node-mongodb-native/api-generated/collection.html#aggregate
* @param {Object|Array} [ops] aggregation operator(s) or operator array
* @api public
*/
...
```

#### <a name="apidoc.element.mongoose.types.Subdocument"></a>[function <span class="apidocSignatureSpan">mongoose.types.</span>Subdocument (value, fields)](#apidoc.element.mongoose.types.Subdocument)
- description and source-code
```javascript
function Subdocument(value, fields) {
  this.$isSingleNested = true;
  Document.call(this, value, fields);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.utils"></a>[module mongoose.utils](#apidoc.module.mongoose.utils)

#### <a name="apidoc.element.mongoose.utils.PopulateOptions"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>PopulateOptions (path, select, match, options, model, subPopulate)](#apidoc.element.mongoose.utils.PopulateOptions)
- description and source-code
```javascript
function PopulateOptions(path, select, match, options, model, subPopulate) {
  this.path = path;
  this.match = match;
  this.select = select;
  this.options = options;
  this.model = model;
  if (typeof subPopulate === 'object') {
    this.populate = subPopulate;
  }
  this._docs = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.utils.args"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>args (args, slice, sliceEnd)](#apidoc.element.mongoose.utils.args)
- description and source-code
```javascript
args = function (args, slice, sliceEnd) {
  var ret = [];
  var len = args.length;

  if (0 === len) return ret;

  var start = slice < 0
    ? Math.max(0, slice + len)
    : slice || 0;

  if (sliceEnd !== undefined) {
    len = sliceEnd < 0
      ? sliceEnd + len
      : sliceEnd
  }

  while (len-- > start) {
    ret[len - start] = args[len];
  }

  return ret;
}
```
- example usage
```shell
...
 * @return {Aggregate}
 * @api public
 */

Aggregate.prototype.append = function() {
var args = (arguments.length === 1 && util.isArray(arguments[0]))
    ? arguments[0]
    : utils.args(arguments);

if (!args.every(isOperator)) {
  throw new Error('Arguments must be aggregate pipeline operators');
}

this._pipeline = this._pipeline.concat(args);
...
```

#### <a name="apidoc.element.mongoose.utils.clone"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>clone (obj, options)](#apidoc.element.mongoose.utils.clone)
- description and source-code
```javascript
function clone(obj, options) {
  if (obj === undefined || obj === null) {
    return obj;
  }

  if (Array.isArray(obj)) {
    return cloneArray(obj, options);
  }

  if (isMongooseObject(obj)) {
    if (options && options.json && typeof obj.toJSON === 'function') {
      return obj.toJSON(options);
    }
    return obj.toObject(options);
  }

  if (obj.constructor) {
    switch (exports.getFunctionName(obj.constructor)) {
      case 'Object':
        return cloneObject(obj, options);
      case 'Date':
        return new obj.constructor(+obj);
      case 'RegExp':
        return cloneRegExp(obj);
      default:
        // ignore
        break;
    }
  }

  if (obj instanceof ObjectId) {
    return new ObjectId(obj.id);
  }
  if (obj instanceof Decimal) {
    if (options && options.flattenDecimals) {
      return obj.toJSON();
    }
    return Decimal.fromString(obj.toString());
  }

  if (!obj.constructor && exports.isObject(obj)) {
    // object created with Object.create(null)
    return cloneObject(obj, options);
  }

  if (obj.valueOf) {
    return obj.valueOf();
  }
}
```
- example usage
```shell
...

Aggregate.prototype.exec = function(callback) {
if (!this._model) {
  throw new Error('Aggregate not bound to any Model');
}
var _this = this;
var Promise = PromiseProvider.get();
var options = utils.clone(this.options);

if (options && options.cursor) {
  if (options.cursor.async) {
    delete options.cursor.async;
    return new Promise.ES6(function(resolve) {
      if (!_this._model.collection.buffer) {
        process.nextTick(function() {
...
```

#### <a name="apidoc.element.mongoose.utils.decorate"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>decorate (destination, source)](#apidoc.element.mongoose.utils.decorate)
- description and source-code
```javascript
decorate = function (destination, source) {
  for (var key in source) {
    destination[key] = source[key];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.utils.deepEqual"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>deepEqual (a, b)](#apidoc.element.mongoose.utils.deepEqual)
- description and source-code
```javascript
function deepEqual(a, b) {
  if (a === b) {
    return true;
  }

  if (a instanceof Date && b instanceof Date) {
    return a.getTime() === b.getTime();
  }

  if ((a instanceof ObjectId && b instanceof ObjectId) ||
      (a instanceof Decimal && b instanceof Decimal)) {
    return a.toString() === b.toString();
  }

  if (a instanceof RegExp && b instanceof RegExp) {
    return a.source === b.source &&
        a.ignoreCase === b.ignoreCase &&
        a.multiline === b.multiline &&
        a.global === b.global;
  }

  if (typeof a !== 'object' && typeof b !== 'object') {
    return a == b;
  }

  if (a === null || b === null || a === undefined || b === undefined) {
    return false;
  }

  if (a.prototype !== b.prototype) {
    return false;
  }

  // Handle MongooseNumbers
  if (a instanceof Number && b instanceof Number) {
    return a.valueOf() === b.valueOf();
  }

  if (Buffer.isBuffer(a)) {
    return exports.buffer.areEqual(a, b);
  }

  if (isMongooseObject(a)) {
    a = a.toObject();
  }
  if (isMongooseObject(b)) {
    b = b.toObject();
  }

  try {
    var ka = Object.keys(a),
        kb = Object.keys(b),
        key, i;
  } catch (e) {
    // happens when one is a string literal and the other isn't
    return false;
  }

  // having the same number of owned properties (keys incorporates
  // hasOwnProperty)
  if (ka.length !== kb.length) {
    return false;
  }

  // the same set of keys (although not necessarily the same order),
  ka.sort();
  kb.sort();

  // ~~~cheap key test
  for (i = ka.length - 1; i >= 0; i--) {
    if (ka[i] !== kb[i]) {
      return false;
    }
  }

  // equivalent values for every corresponding key, and
  // ~~~possibly expensive deep test
  for (i = ka.length - 1; i >= 0; i--) {
    key = ka[i];
    if (!deepEqual(a[key], b[key])) {
      return false;
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.utils.each"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>each (arr, fn)](#apidoc.element.mongoose.utils.each)
- description and source-code
```javascript
each = function (arr, fn) {
  for (var i = 0; i < arr.length; ++i) {
    fn(arr[i]);
  }
}
```
- example usage
```shell
...
* Sets the cursor option option for the aggregation query (ignored for < 2.6.0).
* Note the different syntax below: .exec() returns a cursor object, and no callback
* is necessary.
*
* ####Example:
*
*     var cursor = Model.aggregate(..).cursor({ batchSize: 1000 }).exec();
*     cursor.each(function(error, doc) {
*       // use doc
*     });
*
* @param {Object} options set the cursor batch size
* @see mongodb http://mongodb.github.io/node-mongodb-native/2.0/api/AggregationCursor.html
*/
...
```

#### <a name="apidoc.element.mongoose.utils.expires"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>expires (object)](#apidoc.element.mongoose.utils.expires)
- description and source-code
```javascript
function expires(object) {
  if (!(object && object.constructor.name === 'Object')) {
    return;
  }
  if (!('expires' in object)) {
    return;
  }

  var when;
  if (typeof object.expires !== 'string') {
    when = object.expires;
  } else {
    when = Math.round(ms(object.expires) / 1000);
  }
  object.expireAfterSeconds = when;
  delete object.expires;
}
```
- example usage
```shell
...
* @param {Object|Boolean|String} options
* @return {SchemaType} this
* @api public
*/

SchemaType.prototype.index = function(options) {
 this._index = options;
 utils.expires(this._index);
 return this;
};

/**
* Declares an unique index.
*
* ####Example:
...
```

#### <a name="apidoc.element.mongoose.utils.getFunctionName"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>getFunctionName (fn)](#apidoc.element.mongoose.utils.getFunctionName)
- description and source-code
```javascript
getFunctionName = function (fn) {
  if (fn.name) {
    return fn.name;
  }
  return (fn.toString().trim().match(/^function\s*([^\s(]+)/) || [])[1];
}
```
- example usage
```shell
...
  var keys;
  var ki;
  var _this = this;

  // determine if this doc is a result of a query with
  // excluded fields

  if (fields && utils.getFunctionName(fields.constructor) === 'Object') {
keys = Object.keys(fields);
ki = keys.length;

if (ki === 1 && keys[0] === '_id') {
  exclude = !!fields[keys[ki]];
} else {
  while (ki--) {
...
```

#### <a name="apidoc.element.mongoose.utils.getValue"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>getValue (path, obj, map)](#apidoc.element.mongoose.utils.getValue)
- description and source-code
```javascript
getValue = function (path, obj, map) {
  return mpath.get(path, obj, '_doc', map);
}
```
- example usage
```shell
...
// If doc._id is not null or undefined
if (doc._id !== null && doc._id !== undefined &&
  opts && opts.populated && opts.populated.length) {
  var id = String(doc._id);
  for (var i = 0; i < opts.populated.length; ++i) {
    var item = opts.populated[i];
    if (item.isVirtual) {
      this.populated(item.path, utils.getValue(item.path, doc), item);
    } else {
      this.populated(item.path, item._docs[id], item);
    }
  }
}

init(this, doc, this._doc);
...
```

#### <a name="apidoc.element.mongoose.utils.isMongooseObject"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>isMongooseObject (v)](#apidoc.element.mongoose.utils.isMongooseObject)
- description and source-code
```javascript
isMongooseObject = function (v) {
  Document || (Document = require('./document'));
  MongooseArray || (MongooseArray = require('./types').Array);
  MongooseBuffer || (MongooseBuffer = require('./types').Buffer);

  return v instanceof Document ||
      (v && v.isMongooseArray) ||
      (v && v.isMongooseBuffer);
}
```
- example usage
```shell
...
    Array.isArray(value.$geometry.coordinates)) {
  if (value.$maxDistance != null) {
    value.$maxDistance = numbertype.castForQuery(value.$maxDistance);
  }
  if (value.$minDistance != null) {
    value.$minDistance = numbertype.castForQuery(value.$minDistance);
  }
  if (utils.isMongooseObject(value.$geometry)) {
    value.$geometry = value.$geometry.toObject({
      transform: false,
      virtuals: false
    });
  }
  value = value.$geometry.coordinates;
} else if (geo === '$geoWithin') {
...
```

#### <a name="apidoc.element.mongoose.utils.isNullOrUndefined"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>isNullOrUndefined (val)](#apidoc.element.mongoose.utils.isNullOrUndefined)
- description and source-code
```javascript
isNullOrUndefined = function (val) {
  return val === null || val === undefined;
}
```
- example usage
```shell
...
 * @api private
 */

exports.toObject = function toObject(obj) {
Document || (Document = require('./document'));
var ret;

if (exports.isNullOrUndefined(obj)) {
  return obj;
}

if (obj instanceof Document) {
  return obj.toObject();
}
...
```

#### <a name="apidoc.element.mongoose.utils.isObject"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>isObject (arg)](#apidoc.element.mongoose.utils.isObject)
- description and source-code
```javascript
isObject = function (arg) {
  if (Buffer.isBuffer(arg)) {
    return true;
  }
  return toString.call(arg) === '[object Object]';
}
```
- example usage
```shell
...
 * @return {Aggregate}
 * @api public
 */

Aggregate.prototype.graphLookup = function(options) {
  var cloneOptions = {};
  if (options) {
if (!utils.isObject(options)) {
  throw new TypeError('Invalid graphLookup() argument. Must be an object.');
}

utils.mergeClone(cloneOptions, options);
var startWith = cloneOptions.startWith;

if (startWith && typeof startWith === 'string') {
...
```

#### <a name="apidoc.element.mongoose.utils.merge"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>merge (to, from, options)](#apidoc.element.mongoose.utils.merge)
- description and source-code
```javascript
function merge(to, from, options) {
  options = options || {};
  var keys = Object.keys(from);
  var i = 0;
  var len = keys.length;
  var key;

  if (options.retainKeyOrder) {
    while (i < len) {
      key = keys[i++];
      if (to[key] == null) {
        to[key] = from[key];
      } else if (exports.isObject(from[key])) {
        merge(to[key], from[key], options);
      } else if (options.overwrite) {
        to[key] = from[key];
      }
    }
  } else {
    while (len--) {
      key = keys[len];
      if (to[key] == null) {
        to[key] = from[key];
      } else if (exports.isObject(from[key])) {
        merge(to[key], from[key], options);
      } else if (options.overwrite) {
        to[key] = from[key];
      }
    }
  }
}
```
- example usage
```shell
...
};

if (isVirtual && virtual.options && virtual.options.options) {
  currentOptions.options = utils.clone(virtual.options.options, {
    retainKeyOrder: true
  });
}
utils.merge(currentOptions, options);
if (schema && !discriminatorKey) {
  currentOptions.model = Model;
}
options.model = Model;

available[modelName] = {
  Model: Model,
...
```

#### <a name="apidoc.element.mongoose.utils.mergeClone"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>mergeClone (to, fromObj)](#apidoc.element.mongoose.utils.mergeClone)
- description and source-code
```javascript
mergeClone = function (to, fromObj) {
  var keys = Object.keys(fromObj);
  var len = keys.length;
  var i = 0;
  var key;

  while (i < len) {
    key = keys[i++];
    if (typeof to[key] === 'undefined') {
      // make sure to retain key order here because of a bug handling the $each
      // operator in mongodb 2.4.4
      to[key] = exports.clone(fromObj[key], {retainKeyOrder: 1});
    } else {
      if (exports.isObject(fromObj[key])) {
        var obj = fromObj[key];
        if (isMongooseObject(fromObj[key]) && !fromObj[key].isMongooseBuffer) {
          obj = obj.toObject({ transform: false, virtuals: false });
        }
        if (fromObj[key].isMongooseBuffer) {
          obj = new Buffer(obj);
        }
        exports.mergeClone(to[key], obj);
      } else {
        // make sure to retain key order here because of a bug handling the
        // $each operator in mongodb 2.4.4
        to[key] = exports.clone(fromObj[key], {retainKeyOrder: 1});
      }
    }
  }
}
```
- example usage
```shell
...
Aggregate.prototype.graphLookup = function(options) {
  var cloneOptions = {};
  if (options) {
if (!utils.isObject(options)) {
  throw new TypeError('Invalid graphLookup() argument. Must be an object.');
}

utils.mergeClone(cloneOptions, options);
var startWith = cloneOptions.startWith;

if (startWith && typeof startWith === 'string') {
  cloneOptions.startWith = cloneOptions.startWith.charAt(0) === '$' ?
    cloneOptions.startWith :
    '$' + cloneOptions.startWith;
}
...
```

#### <a name="apidoc.element.mongoose.utils.options"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>options (defaults, options)](#apidoc.element.mongoose.utils.options)
- description and source-code
```javascript
options = function (defaults, options) {
  var keys = Object.keys(defaults),
      i = keys.length,
      k;

  options = options || {};

  while (i--) {
    k = keys[i];
    if (!(k in options)) {
      options[k] = defaults[k];
    }
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose.utils.populate"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>populate (path, select, model, match, options, subPopulate)](#apidoc.element.mongoose.utils.populate)
- description and source-code
```javascript
function populate(path, select, model, match, options, subPopulate) {
  // The order of select/conditions args is opposite Model.find but
  // necessary to keep backward compatibility (select could be
  // an array, string, or object literal).

  // might have passed an object specifying all arguments
  if (arguments.length === 1) {
    if (path instanceof PopulateOptions) {
      return [path];
    }

    if (Array.isArray(path)) {
      return path.map(function(o) {
        return exports.populate(o)[0];
      });
    }

    if (exports.isObject(path)) {
      match = path.match;
      options = path.options;
      select = path.select;
      model = path.model;
      subPopulate = path.populate;
      path = path.path;
    }
  } else if (typeof model !== 'string' && typeof model !== 'function') {
    options = match;
    match = model;
    model = undefined;
  }

  if (typeof path !== 'string') {
    throw new TypeError('utils.populate: invalid path. Expected string. Got typeof '' + typeof path + ''');
  }

  if (typeof subPopulate === 'object') {
    subPopulate = exports.populate(subPopulate);
  }

  var ret = [];
  var paths = path.split(' ');
  options = exports.clone(options, { retainKeyOrder: true });
  for (var i = 0; i < paths.length; ++i) {
    ret.push(new PopulateOptions(paths[i], select, match, options, model, subPopulate));
  }

  return ret;
}
```
- example usage
```shell
...
* Populates document references, executing the 'callback' when complete.
* If you want to use promises instead, use this function with
* ['execPopulate()'](#document_Document-execPopulate)
*
* ####Example:
*
*     doc
*     .populate('company')
*     .populate({
*       path: 'notes',
*       match: /airline/,
*       select: 'text',
*       model: 'modelName'
*       options: opts
*     }, function (err, user) {
...
```

#### <a name="apidoc.element.mongoose.utils.random"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>random ()](#apidoc.element.mongoose.utils.random)
- description and source-code
```javascript
random = function () {
  return Math.random().toString().substr(3);
}
```
- example usage
```shell
...
/*!
* Generates a random string
*
* @api private
*/

exports.random = function() {
 return Math.random().toString().substr(3);
};

/*!
* Merges 'from' into 'to' without overwriting existing properties.
*
* @param {Object} to
* @param {Object} from
...
```

#### <a name="apidoc.element.mongoose.utils.setValue"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>setValue (path, val, obj, map)](#apidoc.element.mongoose.utils.setValue)
- description and source-code
```javascript
setValue = function (path, val, obj, map) {
  mpath.set(path, val, obj, '_doc', map);
}
```
- example usage
```shell
...
  }

  var pathType = this.schema.pathType(path);
  if (pathType === 'nested' && val) {
    if (utils.isObject(val) &&
  (!val.constructor || utils.getFunctionName(val.constructor) === 'Object')) {
if (!merge) {
  this.setValue(path, null);
  cleanModifiedSubpaths(this, path);
}

if (Object.keys(val).length === 0) {
  this.setValue(path, {});
  this.markModified(path);
  cleanModifiedSubpaths(this, path);
...
```

#### <a name="apidoc.element.mongoose.utils.tick"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>tick (callback)](#apidoc.element.mongoose.utils.tick)
- description and source-code
```javascript
function tick(callback) {
  if (typeof callback !== 'function') {
    return;
  }
  return function() {
    try {
      callback.apply(this, arguments);
    } catch (err) {
      // only nextTick on err to get out of
      // the event loop and avoid state corruption.
      process.nextTick(function() {
        throw err;
      });
    }
  };
}
```
- example usage
```shell
...

  var indexFields = index[0];
  var options = index[1];
  _handleSafe(options);

  indexSingleStart(indexFields, options);

  model.collection.ensureIndex(indexFields, options, utils.tick(function(err, name) {
    indexSingleDone(err, indexFields, options, name);
    if (err) {
      return done(err);
    }
    create();
  }));
};
...
```

#### <a name="apidoc.element.mongoose.utils.toCollectionName"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>toCollectionName (name, options)](#apidoc.element.mongoose.utils.toCollectionName)
- description and source-code
```javascript
toCollectionName = function (name, options) {
  options = options || {};
  if (name === 'system.profile') {
    return name;
  }
  if (name === 'system.indexes') {
    return name;
  }
  if (options.pluralization === false) {
    return name;
  }
  return pluralize(name.toLowerCase());
}
```
- example usage
```shell
...
    ? schema
    : _this.prototype.schema;

var options = s.options || {};

if (!collection) {
  collection = _this.prototype.schema.get('collection')
      || utils.toCollectionName(_this.modelName, options);
}

var collectionOptions = {
  bufferCommands: s ? options.bufferCommands : true,
  capped: s && options.capped
};
...
```

#### <a name="apidoc.element.mongoose.utils.toObject"></a>[function <span class="apidocSignatureSpan">mongoose.utils.</span>toObject (obj)](#apidoc.element.mongoose.utils.toObject)
- description and source-code
```javascript
function toObject(obj) {
  Document || (Document = require('./document'));
  var ret;

  if (exports.isNullOrUndefined(obj)) {
    return obj;
  }

  if (obj instanceof Document) {
    return obj.toObject();
  }

  if (Array.isArray(obj)) {
    ret = [];

    for (var i = 0, len = obj.length; i < len; ++i) {
      ret.push(toObject(obj[i]));
    }

    return ret;
  }

  if ((obj.constructor && exports.getFunctionName(obj.constructor) === 'Object') ||
      (!obj.constructor && exports.isObject(obj))) {
    ret = {};

    for (var k in obj) {
      ret[k] = toObject(obj[k]);
    }

    return ret;
  }

  return obj;
}
```
- example usage
```shell
...
  if (value.$maxDistance != null) {
    value.$maxDistance = numbertype.castForQuery(value.$maxDistance);
  }
  if (value.$minDistance != null) {
    value.$minDistance = numbertype.castForQuery(value.$minDistance);
  }
  if (utils.isMongooseObject(value.$geometry)) {
    value.$geometry = value.$geometry.toObject({
      transform: false,
      virtuals: false
    });
  }
  value = value.$geometry.coordinates;
} else if (geo === '$geoWithin') {
  if (value.$geometry) {
...
```



# <a name="apidoc.module.mongoose.virtualtype"></a>[module mongoose.virtualtype](#apidoc.module.mongoose.virtualtype)

#### <a name="apidoc.element.mongoose.virtualtype.virtualtype"></a>[function <span class="apidocSignatureSpan">mongoose.</span>virtualtype (options, name)](#apidoc.element.mongoose.virtualtype.virtualtype)
- description and source-code
```javascript
function VirtualType(options, name) {
  this.path = name;
  this.getters = [];
  this.setters = [];
  this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose.virtualtype.prototype"></a>[module mongoose.virtualtype.prototype](#apidoc.module.mongoose.virtualtype.prototype)

#### <a name="apidoc.element.mongoose.virtualtype.prototype.applyGetters"></a>[function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>applyGetters (value, scope)](#apidoc.element.mongoose.virtualtype.prototype.applyGetters)
- description and source-code
```javascript
applyGetters = function (value, scope) {
  var v = value;
  for (var l = this.getters.length - 1; l >= 0; l--) {
    v = this.getters[l].call(scope, v, this);
  }
  return v;
}
```
- example usage
```shell
...
 if (adhoc) {
   obj = adhoc.cast(obj);
 }

 // Check if this path is populated - don't apply getters if it is,
 // because otherwise its a nested object. See gh-3357
 if (schema && !this.populated(path)) {
   obj = schema.applyGetters(obj, this);
 }

 return obj;
};

/**
* Returns the schematype for the given 'path'.
...
```

#### <a name="apidoc.element.mongoose.virtualtype.prototype.applySetters"></a>[function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>applySetters (value, scope)](#apidoc.element.mongoose.virtualtype.prototype.applySetters)
- description and source-code
```javascript
applySetters = function (value, scope) {
  var v = value;
  for (var l = this.setters.length - 1; l >= 0; l--) {
    v = this.setters[l].call(scope, v, this);
  }
  return v;
}
```
- example usage
```shell
...
    if (strict === 'throw') {
      throw new StrictModeError(path);
    }
    return this;
  }
} else if (pathType === 'virtual') {
  schema = this.schema.virtualpath(path);
  schema.applySetters(val, this);
  return this;
} else {
  schema = this.$__path(path);
}

var pathToMark;
...
```

#### <a name="apidoc.element.mongoose.virtualtype.prototype.get"></a>[function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>get (fn)](#apidoc.element.mongoose.virtualtype.prototype.get)
- description and source-code
```javascript
get = function (fn) {
  this.getters.push(fn);
  return this;
}
```
- example usage
```shell
...
// a setter
Comment.path('name').set(function (v) {
  return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
  notify(this.get('email'));
  next();
});
'''

Take a look at the example in 'examples/schema.js' for an end-to-end example of a typical setup.

### Accessing a Model
...
```

#### <a name="apidoc.element.mongoose.virtualtype.prototype.set"></a>[function <span class="apidocSignatureSpan">mongoose.virtualtype.prototype.</span>set (fn)](#apidoc.element.mongoose.virtualtype.prototype.set)
- description and source-code
```javascript
set = function (fn) {
  this.setters.push(fn);
  return this;
}
```
- example usage
```shell
...
age: { type: Number, min: 18, index: true },
bio: { type: String, match: /[a-z]/ },
date: { type: Date, default: Date.now },
buff: Buffer
});

// a setter
Comment.path('name').set(function (v) {
return capitalize(v);
});

// middleware
Comment.pre('save', function (next) {
notify(this.get('email'));
next();
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
