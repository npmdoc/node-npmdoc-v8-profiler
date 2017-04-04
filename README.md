# api documentation for  [v8-profiler (v5.7.0)](http://github.com/node-inspector/v8-profiler)  [![npm package](https://img.shields.io/npm/v/npmdoc-v8-profiler.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-v8-profiler) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-v8-profiler.svg)](https://travis-ci.org/npmdoc/node-npmdoc-v8-profiler)
#### node bindings for the v8 profiler

[![NPM](https://nodei.co/npm/v8-profiler.png?downloads=true)](https://www.npmjs.com/package/v8-profiler)

[![apidoc](https://npmdoc.github.io/node-npmdoc-v8-profiler/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-v8-profiler_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-v8-profiler/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-v8-profiler/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-v8-profiler/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Danny Coates",
        "email": "dannycoates@gmail.com"
    },
    "binary": {
        "module_name": "profiler",
        "module_path": "./build/{module_name}/v{version}/{node_abi}-{platform}-{arch}/",
        "remote_path": "./{module_name}/v{version}/",
        "package_name": "{node_abi}-{platform}-{arch}.tar.gz",
        "host": "https://node-inspector.s3.amazonaws.com/"
    },
    "bugs": {
        "url": "https://github.com/node-inspector/v8-profiler/issues"
    },
    "contributors": [
        {
            "name": "Miroslav Bajtoš"
        },
        {
            "name": "3y3",
            "email": "3y3@bk.ru"
        }
    ],
    "dependencies": {
        "nan": "^2.5.1",
        "node-pre-gyp": "^0.6.34"
    },
    "description": "node bindings for the v8 profiler",
    "devDependencies": {
        "aws-sdk": "^2.0.0",
        "chai": "^1.9.1",
        "co": "^4.6.0",
        "mocha": "^1.20.1",
        "rimraf": "^2.4.4"
    },
    "directories": {},
    "dist": {
        "shasum": "e8381cbebb5b5fd0ca8d2b09f6a0181a158db34d",
        "tarball": "https://registry.npmjs.org/v8-profiler/-/v8-profiler-5.7.0.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "ce5bbb902821f56b628936f4fa5fc9c6d8b4a655",
    "homepage": "http://github.com/node-inspector/v8-profiler",
    "keywords": [
        "profiler",
        "inspector"
    ],
    "license": "BSD-2-Clause",
    "main": "v8-profiler",
    "maintainers": [
        {
            "name": "dannycoates",
            "email": "dannycoates@gmail.com"
        },
        {
            "name": "bajtos",
            "email": "miro.bajtos@gmail.com"
        },
        {
            "name": "3y3",
            "email": "3y3@bk.ru"
        }
    ],
    "name": "v8-profiler",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/node-inspector/v8-profiler.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "preinstall": "node -e 'process.exit(0)'",
        "rebuild": "node-pre-gyp rebuild",
        "release": "node ./tools/release.js $@",
        "test": "mocha --debug"
    },
    "version": "5.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module v8-profiler](#apidoc.module.v8-profiler)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>annotate_tag ()](#apidoc.element.v8-profiler.annotate_tag)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>deleteAllProfiles ()](#apidoc.element.v8-profiler.deleteAllProfiles)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>deleteAllSnapshots ()](#apidoc.element.v8-profiler.deleteAllSnapshots)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>getHeapObjectId (value)](#apidoc.element.v8-profiler.getHeapObjectId)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>getHeapStats (iterator, callback)](#apidoc.element.v8-profiler.getHeapStats)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>getObjectByHeapObjectId (id)](#apidoc.element.v8-profiler.getObjectByHeapObjectId)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>history ()](#apidoc.element.v8-profiler.history)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>prepublish_to_npm ()](#apidoc.element.v8-profiler.prepublish_to_npm)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>setSamplingInterval (num)](#apidoc.element.v8-profiler.setSamplingInterval)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>startProfiling (name, recsamples)](#apidoc.element.v8-profiler.startProfiling)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>startTrackingHeapObjects ()](#apidoc.element.v8-profiler.startTrackingHeapObjects)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>stopProfiling (name)](#apidoc.element.v8-profiler.stopProfiling)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>stopTrackingHeapObjects ()](#apidoc.element.v8-profiler.stopTrackingHeapObjects)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>takeSnapshot (name, control)](#apidoc.element.v8-profiler.takeSnapshot)
1.  object <span class="apidocSignatureSpan">v8-profiler.</span>profiles
1.  object <span class="apidocSignatureSpan">v8-profiler.</span>snapshots

#### [module v8-profiler.annotate_tag](#apidoc.module.v8-profiler.annotate_tag)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>annotate_tag ()](#apidoc.element.v8-profiler.annotate_tag.annotate_tag)
1.  [function <span class="apidocSignatureSpan">v8-profiler.annotate_tag.</span>__generatorFunction__ (version)](#apidoc.element.v8-profiler.annotate_tag.__generatorFunction__)

#### [module v8-profiler.history](#apidoc.module.v8-profiler.history)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>history ()](#apidoc.element.v8-profiler.history.history)
1.  [function <span class="apidocSignatureSpan">v8-profiler.history.</span>__generatorFunction__ ()](#apidoc.element.v8-profiler.history.__generatorFunction__)

#### [module v8-profiler.prepublish_to_npm](#apidoc.module.v8-profiler.prepublish_to_npm)
1.  [function <span class="apidocSignatureSpan">v8-profiler.</span>prepublish_to_npm ()](#apidoc.element.v8-profiler.prepublish_to_npm.prepublish_to_npm)
1.  [function <span class="apidocSignatureSpan">v8-profiler.prepublish_to_npm.</span>__generatorFunction__ ()](#apidoc.element.v8-profiler.prepublish_to_npm.__generatorFunction__)



# <a name="apidoc.module.v8-profiler"></a>[module v8-profiler](#apidoc.module.v8-profiler)

#### <a name="apidoc.element.v8-profiler.annotate_tag"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>annotate_tag ()](#apidoc.element.v8-profiler.annotate_tag)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.deleteAllProfiles"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>deleteAllProfiles ()](#apidoc.element.v8-profiler.deleteAllProfiles)
- description and source-code
```javascript
deleteAllProfiles = function () {
  Object.keys(binding.cpu.profiles).forEach(function(key) {
    binding.cpu.profiles[key].delete();
  });
}
```
- example usage
```shell
...

'deleteAllProfiles()' - works as described in name.

'''js
profiler.startProfiling('', true);
setTimeout(function() {
  var profile = profiler.stopProfiling('');
  profiler.deleteAllProfiles();
}, 1000);
'''

### HEAP Snapshot API
'Snapshot.getHeader()' - provides short information about snapshot.

'Snapshot.compare(snapshot)' - creates HEAP diff for two snapshots.
...
```

#### <a name="apidoc.element.v8-profiler.deleteAllSnapshots"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>deleteAllSnapshots ()](#apidoc.element.v8-profiler.deleteAllSnapshots)
- description and source-code
```javascript
deleteAllSnapshots = function () {
  Object.keys(binding.heap.snapshots).forEach(function(key) {
    binding.heap.snapshots[key].delete();
  });
}
```
- example usage
```shell
...
'takeSnapshot([name])' - returns new HEAP Snapshot instance. 'name' is optional argument, by default snapshot name will be constructed
 from his uid.

'deleteAllSnapshots()' - works as described in name.

'''js
var snapshot1 = profiler.takeSnapshot('1');
var snapshot2 = profiler.takeSnapshot();
profiler.deleteAllSnapshots();
'''

'startProfiling([name], [recsamples])' - start CPU profiling. 'name' is optional argument, by default profile name will be constructed
 from his uid. 'recsamples' is true by default.

'stopProfiling([name])' - returns new CPU Profile instance. There is no strictly described behavior for usage without 'name' argument
.

'setSamplingInterval([num])' - Changes default CPU profiler sampling interval to the specified number of microseconds. Default interval
 is 1000us. This method must be called when there are no profiles being recorded. If called without arguments it resets interval
 to default.
...
```

#### <a name="apidoc.element.v8-profiler.getHeapObjectId"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>getHeapObjectId (value)](#apidoc.element.v8-profiler.getHeapObjectId)
- description and source-code
```javascript
getHeapObjectId = function (value) {
  if (!arguments.length) return;
  return binding.heap.getHeapObjectId(value);
}
```
- example usage
```shell
...
  if (isNaN(id)) return;

  return binding.heap.getObjectByHeapObjectId(id);
},

getHeapObjectId: function(value) {
  if (!arguments.length) return;
  return binding.heap.getHeapObjectId(value);
},

/*CPU PROFILER API*/

get profiles() { return binding.cpu.profiles; },

startProfiling: function(name, recsamples) {
...
```

#### <a name="apidoc.element.v8-profiler.getHeapStats"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>getHeapStats (iterator, callback)](#apidoc.element.v8-profiler.getHeapStats)
- description and source-code
```javascript
getHeapStats = function (iterator, callback) {
  if (typeof iterator !== 'function')
    iterator = function noop() {};

  if (typeof callback !== 'function')
    callback = function noop() {};

  return binding.heap.getHeapStats(iterator, callback)
}
```
- example usage
```shell
...
  getHeapStats: function(iterator, callback) {
if (typeof iterator !== 'function')
  iterator = function noop() {};

if (typeof callback !== 'function')
  callback = function noop() {};

return binding.heap.getHeapStats(iterator, callback)
  },

  getObjectByHeapObjectId: function(id) {
id = parseInt(id, 10);
if (isNaN(id)) return;

return binding.heap.getObjectByHeapObjectId(id);
...
```

#### <a name="apidoc.element.v8-profiler.getObjectByHeapObjectId"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>getObjectByHeapObjectId (id)](#apidoc.element.v8-profiler.getObjectByHeapObjectId)
- description and source-code
```javascript
getObjectByHeapObjectId = function (id) {
  id = parseInt(id, 10);
  if (isNaN(id)) return;

  return binding.heap.getObjectByHeapObjectId(id);
}
```
- example usage
```shell
...
  return binding.heap.getHeapStats(iterator, callback)
},

getObjectByHeapObjectId: function(id) {
  id = parseInt(id, 10);
  if (isNaN(id)) return;

  return binding.heap.getObjectByHeapObjectId(id);
},

getHeapObjectId: function(value) {
  if (!arguments.length) return;
  return binding.heap.getHeapObjectId(value);
},
...
```

#### <a name="apidoc.element.v8-profiler.history"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>history ()](#apidoc.element.v8-profiler.history)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.prepublish_to_npm"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>prepublish_to_npm ()](#apidoc.element.v8-profiler.prepublish_to_npm)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.setSamplingInterval"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>setSamplingInterval (num)](#apidoc.element.v8-profiler.setSamplingInterval)
- description and source-code
```javascript
setSamplingInterval = function (num) {
  if (activeProfiles.length) {
    throw new Error('setSamplingInterval must be called when there are no profiles being recorded.');
  }

  num = parseInt(num, 10) || 1000;
  binding.cpu.setSamplingInterval(num);
}
```
- example usage
```shell
...

setSamplingInterval: function(num) {
  if (activeProfiles.length) {
    throw new Error('setSamplingInterval must be called when there are no profiles being recorded.');
  }

  num = parseInt(num, 10) || 1000;
  binding.cpu.setSamplingInterval(num);
},

deleteAllProfiles: function() {
  Object.keys(binding.cpu.profiles).forEach(function(key) {
    binding.cpu.profiles[key].delete();
  });
}
...
```

#### <a name="apidoc.element.v8-profiler.startProfiling"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>startProfiling (name, recsamples)](#apidoc.element.v8-profiler.startProfiling)
- description and source-code
```javascript
startProfiling = function (name, recsamples) {
  if (activeProfiles.length == 0 && typeof process._startProfilerIdleNotifier == "function")
    process._startProfilerIdleNotifier();

  if (typeof name == 'boolean') {
    recsamples = name;
    name = '';
  }

  recsamples = recsamples === undefined ? true : Boolean(recsamples);
  name = '' + name;

  if (activeProfiles.indexOf(name) < 0)
    activeProfiles.push(name)

  startTime = Date.now();
  binding.cpu.startProfiling(name, recsamples);
}
```
- example usage
```shell
...
'stopProfiling([name])' - returns new CPU Profile instance. There is no strictly described behavior for usage without 'name' argument
.

'setSamplingInterval([num])' - Changes default CPU profiler sampling interval to the specified number of microseconds. Default interval
 is 1000us. This method must be called when there are no profiles being recorded. If called without arguments it resets interval
 to default.

'deleteAllProfiles()' - works as described in name.

'''js
profiler.startProfiling('', true);
setTimeout(function() {
  var profile = profiler.stopProfiling('');
  profiler.deleteAllProfiles();
}, 1000);
'''

### HEAP Snapshot API
...
```

#### <a name="apidoc.element.v8-profiler.startTrackingHeapObjects"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>startTrackingHeapObjects ()](#apidoc.element.v8-profiler.startTrackingHeapObjects)
- description and source-code
```javascript
startTrackingHeapObjects = function () {
  binding.heap.startTrackingHeapObjects();
}
```
- example usage
```shell
...
deleteAllSnapshots: function () {
  Object.keys(binding.heap.snapshots).forEach(function(key) {
    binding.heap.snapshots[key].delete();
  });
},

startTrackingHeapObjects: function() {
  binding.heap.startTrackingHeapObjects();
},

stopTrackingHeapObjects: function() {
  binding.heap.stopTrackingHeapObjects();
},

getHeapStats: function(iterator, callback) {
...
```

#### <a name="apidoc.element.v8-profiler.stopProfiling"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>stopProfiling (name)](#apidoc.element.v8-profiler.stopProfiling)
- description and source-code
```javascript
stopProfiling = function (name) {
  var index = activeProfiles.indexOf(name);
  if (name && index < 0)
    return;

  var profile = binding.cpu.stopProfiling(name);
  endTime = Date.now();
  profile.__proto__ = CpuProfile.prototype;
  if (!profile.startTime) profile.startTime = startTime;
  if (!profile.endTime) profile.endTime = endTime;

  if (name)
    activeProfiles.splice(index, 1);
  else
    activeProfiles.length = activeProfiles.length - 1;

  if (activeProfiles.length == 0 && typeof process._stopProfilerIdleNotifier == "function")
    process._stopProfilerIdleNotifier();

  return profile;
}
```
- example usage
```shell
...
'setSamplingInterval([num])' - Changes default CPU profiler sampling interval to the specified number of microseconds. Default interval
 is 1000us. This method must be called when there are no profiles being recorded. If called without arguments it resets interval
 to default.

'deleteAllProfiles()' - works as described in name.

'''js
profiler.startProfiling('', true);
setTimeout(function() {
  var profile = profiler.stopProfiling('');
  profiler.deleteAllProfiles();
}, 1000);
'''

### HEAP Snapshot API
'Snapshot.getHeader()' - provides short information about snapshot.
...
```

#### <a name="apidoc.element.v8-profiler.stopTrackingHeapObjects"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>stopTrackingHeapObjects ()](#apidoc.element.v8-profiler.stopTrackingHeapObjects)
- description and source-code
```javascript
stopTrackingHeapObjects = function () {
  binding.heap.stopTrackingHeapObjects();
}
```
- example usage
```shell
...
  },

  startTrackingHeapObjects: function() {
binding.heap.startTrackingHeapObjects();
  },

  stopTrackingHeapObjects: function() {
binding.heap.stopTrackingHeapObjects();
  },

  getHeapStats: function(iterator, callback) {
if (typeof iterator !== 'function')
  iterator = function noop() {};

if (typeof callback !== 'function')
...
```

#### <a name="apidoc.element.v8-profiler.takeSnapshot"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>takeSnapshot (name, control)](#apidoc.element.v8-profiler.takeSnapshot)
- description and source-code
```javascript
takeSnapshot = function (name, control) {
  if (typeof name == 'function') {
    control = name;
    name = '';
  }

  if (typeof control !== 'function') {
    control = function noop() {};
  }

  name = '' + name;

  var snapshot = binding.heap.takeSnapshot(name, control);
  snapshot.__proto__ = Snapshot.prototype;
  snapshot.title = name;
  return snapshot;
}
```
- example usage
```shell
...
'''
## API
'takeSnapshot([name])' - returns new HEAP Snapshot instance. 'name' is optional argument, by default snapshot name will be constructed
 from his uid.

'deleteAllSnapshots()' - works as described in name.

'''js
var snapshot1 = profiler.takeSnapshot('1');
var snapshot2 = profiler.takeSnapshot();
profiler.deleteAllSnapshots();
'''

'startProfiling([name], [recsamples])' - start CPU profiling. 'name' is optional argument, by default profile name will be constructed
 from his uid. 'recsamples' is true by default.

'stopProfiling([name])' - returns new CPU Profile instance. There is no strictly described behavior for usage without 'name' argument
.
...
```



# <a name="apidoc.module.v8-profiler.annotate_tag"></a>[module v8-profiler.annotate_tag](#apidoc.module.v8-profiler.annotate_tag)

#### <a name="apidoc.element.v8-profiler.annotate_tag.annotate_tag"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>annotate_tag ()](#apidoc.element.v8-profiler.annotate_tag.annotate_tag)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.annotate_tag.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">v8-profiler.annotate_tag.</span>__generatorFunction__ (version)](#apidoc.element.v8-profiler.annotate_tag.__generatorFunction__)
- description and source-code
```javascript
function* (version) {
  const history = yield require('./history')(version);
  const tagname = 'v' + version;

  return yield exec('git tag -a "' + tagname + '" -m "' + history + '"');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.v8-profiler.history"></a>[module v8-profiler.history](#apidoc.module.v8-profiler.history)

#### <a name="apidoc.element.v8-profiler.history.history"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>history ()](#apidoc.element.v8-profiler.history.history)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.history.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">v8-profiler.history.</span>__generatorFunction__ ()](#apidoc.element.v8-profiler.history.__generatorFunction__)
- description and source-code
```javascript
function* () {
  const _lasttag = yield exec('git rev-list --tags --max-count=1');
  const _version = yield exec('git describe --tags --abbrev=0 ' + _lasttag);
  const version = _version ? ' ' + _version + '..' : '';

  return ' ' + (yield exec('git log --no-merges --pretty="format: * %s (%an) %H%n"' + version));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.v8-profiler.prepublish_to_npm"></a>[module v8-profiler.prepublish_to_npm](#apidoc.module.v8-profiler.prepublish_to_npm)

#### <a name="apidoc.element.v8-profiler.prepublish_to_npm.prepublish_to_npm"></a>[function <span class="apidocSignatureSpan">v8-profiler.</span>prepublish_to_npm ()](#apidoc.element.v8-profiler.prepublish_to_npm.prepublish_to_npm)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.v8-profiler.prepublish_to_npm.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">v8-profiler.prepublish_to_npm.</span>__generatorFunction__ ()](#apidoc.element.v8-profiler.prepublish_to_npm.__generatorFunction__)
- description and source-code
```javascript
function* () {
  rimraf.sync('./build');

  const targets = [];
  Object.keys(matrix).forEach(
    (arch) => matrix[arch].forEach(
    (platform) => versions.forEach(
    (version) => targets.push(new Target(arch, platform, version))
  )));

  while (targets.length) yield install(targets.pop());
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
