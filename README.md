# api documentation for  [scp2 (v0.5.0)](https://github.com/lepture/node-scp2)  [![npm package](https://img.shields.io/npm/v/npmdoc-scp2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-scp2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-scp2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-scp2)
#### A pure javascript scp program based on ssh2.

[![NPM](https://nodei.co/npm/scp2.png?downloads=true)](https://www.npmjs.com/package/scp2)

[![apidoc](https://npmdoc.github.io/node-npmdoc-scp2/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-scp2_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-scp2/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-scp2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-scp2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Hsiaoming Yang",
        "email": "lepture@me.com"
    },
    "bin": {
        "scp2": "bin/scp2"
    },
    "bugs": {
        "url": "https://github.com/lepture/node-scp2/issues"
    },
    "dependencies": {
        "async": "~0.9.0",
        "glob": "~7.0.3",
        "lodash": "~4.11.1",
        "ssh2": "~0.4.10"
    },
    "description": "A pure javascript scp program based on ssh2.",
    "devDependencies": {
        "expect.js": "0",
        "jscoverage": "^0.5.9",
        "jshint": "2",
        "mocha": "2"
    },
    "directories": {},
    "dist": {
        "shasum": "64ee74bc3685f3a4c6290f2da8c1e3b4eef92e8d",
        "tarball": "https://registry.npmjs.org/scp2/-/scp2-0.5.0.tgz"
    },
    "gitHead": "a710ec8efca78cac0023a4b3dcb21c50ccceb3b9",
    "homepage": "https://github.com/lepture/node-scp2",
    "keywords": [
        "ssh",
        "scp",
        "copy",
        "remote",
        "ssh2"
    ],
    "maintainers": [
        {
            "name": "lepture",
            "email": "sopheryoung@gmail.com"
        },
        {
            "name": "popomore",
            "email": "sakura9515@gmail.com"
        }
    ],
    "name": "scp2",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/lepture/node-scp2.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.5.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module scp2](#apidoc.module.scp2)
1.  [function <span class="apidocSignatureSpan">scp2.</span>Client (options)](#apidoc.element.scp2.Client)
1.  [function <span class="apidocSignatureSpan">scp2.</span>scp (src, dest, client, callback)](#apidoc.element.scp2.scp)
1.  object <span class="apidocSignatureSpan">scp2.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">scp2.</span>_options
1.  object <span class="apidocSignatureSpan">scp2.</span>client
1.  object <span class="apidocSignatureSpan">scp2.</span>remote

#### [module scp2.Client](#apidoc.module.scp2.Client)
1.  [function <span class="apidocSignatureSpan">scp2.</span>Client (options)](#apidoc.element.scp2.Client.Client)
1.  [function <span class="apidocSignatureSpan">scp2.Client.</span>super_ ()](#apidoc.element.scp2.Client.super_)

#### [module scp2.Client.prototype](#apidoc.module.scp2.Client.prototype)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>close ()](#apidoc.element.scp2.Client.prototype.close)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>defaults (options)](#apidoc.element.scp2.Client.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>download (src, dest, callback)](#apidoc.element.scp2.Client.prototype.download)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>mkdir (dir, attrs, callback)](#apidoc.element.scp2.Client.prototype.mkdir)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>parse (remote)](#apidoc.element.scp2.Client.prototype.parse)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>sftp (callback)](#apidoc.element.scp2.Client.prototype.sftp)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>upload (src, dest, callback)](#apidoc.element.scp2.Client.prototype.upload)
1.  [function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>write (options, callback)](#apidoc.element.scp2.Client.prototype.write)

#### [module scp2.client](#apidoc.module.scp2.client)
1.  [function <span class="apidocSignatureSpan">scp2.client.</span>Client (options)](#apidoc.element.scp2.client.Client)
1.  object <span class="apidocSignatureSpan">scp2.client.</span>_options
1.  object <span class="apidocSignatureSpan">scp2.client.</span>remote



# <a name="apidoc.module.scp2"></a>[module scp2](#apidoc.module.scp2)

#### <a name="apidoc.element.scp2.Client"></a>[function <span class="apidocSignatureSpan">scp2.</span>Client (options)](#apidoc.element.scp2.Client)
- description and source-code
```javascript
function Client(options) {
  this._options = options || {};

  this.remote = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scp2.scp"></a>[function <span class="apidocSignatureSpan">scp2.</span>scp (src, dest, client, callback)](#apidoc.element.scp2.scp)
- description and source-code
```javascript
scp = function (src, dest, client, callback) {
  if (typeof client === 'function') {
    callback = client;
    client = new Client();
  }
  client.on('error', callback);
  var parsed = client.parse(src);
  if (parsed.host && parsed.path) {
    cp2local(client, parsed, dest, callback);
  } else {
    cp2remote(client, src, dest, callback);
  }
}
```
- example usage
```shell
...
'''js
var client = require('scp2')
'''

Copy a file to the server:

'''js
client.scp('file.txt', 'admin:password@example.com:/home/admin/', function(err) {
})
'''

You can also add the port to the url (default is 22):

'''js
client.scp('file.txt', 'admin:password@example.com:port:/home/admin/', function(err) {
...
```



# <a name="apidoc.module.scp2.Client"></a>[module scp2.Client](#apidoc.module.scp2.Client)

#### <a name="apidoc.element.scp2.Client.Client"></a>[function <span class="apidocSignatureSpan">scp2.</span>Client (options)](#apidoc.element.scp2.Client.Client)
- description and source-code
```javascript
function Client(options) {
  this._options = options || {};

  this.remote = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scp2.Client.super_"></a>[function <span class="apidocSignatureSpan">scp2.Client.</span>super_ ()](#apidoc.element.scp2.Client.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.scp2.Client.prototype"></a>[module scp2.Client.prototype](#apidoc.module.scp2.Client.prototype)

#### <a name="apidoc.element.scp2.Client.prototype.close"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>close ()](#apidoc.element.scp2.Client.prototype.close)
- description and source-code
```javascript
close = function () {
  if (this.__sftp) {
    this.__sftp.end();
    this.__sftp = null;
  }
  if (this.__ssh) {
    this.__ssh.end();
    this.__ssh = null;
  }
}
```
- example usage
```shell
...
    self.emit('transfer', buf, lastCursor, length);
    sftp.write(handle, buf, 0, buf.length, lastIndex, function(err) {
      lastIndex += buf.length;
      lastCursor += 1;
      callback(err);
    });
  }, function(err) {
    sftp.close(handle, callback);
  });
} else if (typeof content === 'number') {
  // content is a file descriptor
  length = parseInt((attrs.size - 1) / chunkSize, 10) + 1;
  var range = new Array(length);
  async.eachSeries(range, function(pos, callback) {
    chunkSize = Math.min(chunkSize, attrs.size - lastIndex);
...
```

#### <a name="apidoc.element.scp2.Client.prototype.defaults"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>defaults (options)](#apidoc.element.scp2.Client.prototype.defaults)
- description and source-code
```javascript
defaults = function (options) {
  if (options) {
    this._options = options || {};
  } else {
    return this._options;
  }
}
```
- example usage
```shell
...


- **defaults** 'function({})'

set the default values for the remote server.

'''js
client.defaults({
    port: 22,
    host: 'example.com',
    username: 'admin',
    privateKey: '....',
    // password: 'password', (accepts password also)
});
'''
...
```

#### <a name="apidoc.element.scp2.Client.prototype.download"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>download (src, dest, callback)](#apidoc.element.scp2.Client.prototype.download)
- description and source-code
```javascript
download = function (src, dest, callback) {
  var self = this;

  self.sftp(function(err,sftp){
    if (err) {
      return callback(err);
    }

    var sftp_readStream = sftp.createReadStream(src);
    sftp_readStream.on('error', function(err){
      callback(err);
    });
    sftp_readStream.pipe(fs.createWriteStream(dest))
    .on('close',function(){
      self.emit('read', src);
      callback(null);
    })
    .on('error', function(err){
      callback(err);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scp2.Client.prototype.mkdir"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>mkdir (dir, attrs, callback)](#apidoc.element.scp2.Client.prototype.mkdir)
- description and source-code
```javascript
mkdir = function (dir, attrs, callback) {
  if (_.isFunction(attrs)) {
    callback = attrs;
    attrs = undefined;
  }

  if (attrs) {
    attrs.mode = getFolderAttr(process.platform, attrs);
  }

  var self = this;
  var dirs = [];
  var exists = false;

  this.sftp(function(err, sftp) {
    if (err) {
      return callback(err);
    }

    // for record log
    var mkdir = function(dir, callback) {
      self.emit('mkdir', dir);
      sftp.mkdir(dir, attrs, callback);
    };

    async.until(function() {
      return exists;
    }, function(done) {
      // detect if the directory exists
      sftp.stat(dir, function(err, attr) {
        if (err) {
          dirs.push(dir);
          dir = path.dirname(dir);
        } else {
          exists = true;
        }
        done();
      });
    }, function(err) {
      if (err) {
        callback(err);
      } else {
        // just like mkdir -p
        async.eachSeries(dirs.reverse(), mkdir, callback);
      }
    });

  });
}
```
- example usage
```shell
...
if (err) {
  return callback(err);
}

// for record log
var mkdir = function(dir, callback) {
  self.emit('mkdir', dir);
  sftp.mkdir(dir, attrs, callback);
};

async.until(function() {
  return exists;
}, function(done) {
  // detect if the directory exists
  sftp.stat(dir, function(err, attr) {
...
```

#### <a name="apidoc.element.scp2.Client.prototype.parse"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>parse (remote)](#apidoc.element.scp2.Client.prototype.parse)
- description and source-code
```javascript
parse = function (remote) {
  if (_.isString(remote)) {
    // username:password@host:/path/to
    var regex = /^([a-zA-Z0-9\-\.]+)(\:.*)?@([^:]+):([^:]+:)?(.*)?$/;
    var m = remote.match(regex);
    if (!m) return {};
    var ret = {
      username: m[1],
      host: m[3],
    };
    if (m[2]) {
      ret.password = m[2].slice(1);
    }
    if (m.length===6 && m[4]) {
      ret.port = m[4].slice(0,-1);
    }
    if (m.length===6 && m[5]) {
      ret.path = m[5];
    } else if (m.length===5 && m[4]) {
      ret.path = m[4];
    }
    this.remote = ret;
    return ret;
  }
  this.remote = remote;
  return remote;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scp2.Client.prototype.sftp"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>sftp (callback)](#apidoc.element.scp2.Client.prototype.sftp)
- description and source-code
```javascript
sftp = function (callback) {
  if (this.__sftp) {
    callback(null, this.__sftp);
    return;
  }

  var remote = _.defaults(this.remote, this._options);
  if (this.__ssh) {
    this.__ssh.connect(remote);
    return;
  }

  var self = this;
  var ssh = new Connection();
  ssh.on('connect', function() {
    self.emit('connect');
  });
  ssh.on('ready', function() {
    self.emit('ready');

    ssh.sftp(function(err, sftp) {
      if (err) throw err;
      // save for reuse
      self.__sftp = sftp;
      callback(err, sftp);
    });
  });
  ssh.on('error', function(err) {
    self.emit('error', err);
    callback(err);
  });
  ssh.on('end', function() {
    self.emit('end');
  });
  ssh.on('close', function() {
    self.emit('close');
  });
  ssh.on('keyboard-interactive', function(name, instructions, instructionsLang, prompts, finish) {
    self.emit('keyboard-interactive', name, instructions, instructionsLang, prompts, finish);
  });
  ssh.on('change password', function(message, language, done) {
    self.emit('change password', message, language, done);
  });
  ssh.on('tcp connection', function(details, accept, reject) {
    self.emit('tcp connection', details, accept, reject);
  });
  ssh.connect(remote);
  this.__ssh = ssh;
}
```
- example usage
```shell
...
var ssh = new Connection();
ssh.on('connect', function() {
  self.emit('connect');
});
ssh.on('ready', function() {
  self.emit('ready');

  ssh.sftp(function(err, sftp) {
    if (err) throw err;
    // save for reuse
    self.__sftp = sftp;
    callback(err, sftp);
  });
});
ssh.on('error', function(err) {
...
```

#### <a name="apidoc.element.scp2.Client.prototype.upload"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>upload (src, dest, callback)](#apidoc.element.scp2.Client.prototype.upload)
- description and source-code
```javascript
upload = function (src, dest, callback) {
  dest = unixy(dest);

  var self = this;

  async.waterfall([
    function(callback) {
      fs.stat(src, callback);
    },
    function(stat, callback) {
      if (stat.isDirectory()) return callback(new Error('Can not upload a directory'));

      // Get the attributes of the source directory
      fs.stat(path.dirname(src), function(err, dirStat) {
        if(err) return callback(err);
        self.mkdir(path.dirname(dest), dirStat, function(err){ callback(err, stat) });
      });
    },
    function(stat, callback) {
      fs.open(src, 'r', function(err, fd) { callback(err, stat, fd); });
    },
    function(stat, fd, callback) {
      self.write({
        source: src,
        destination: dest,
        content: fd,
        attrs: stat
      }, callback);
    }
  ], function(err) {
    callback(err);
  });
}
```
- example usage
```shell
...
- source: the source path, e.g. local/file.txt

- **upload** 'function(src, dest, callback) -> callback(err)'

upload a local file to the server.

'''js
client.upload('file.txt', '/home/admin/file.txt', callback)
'''

- **download** 'function(src, dest, callback) -> callback(err)'

download a server file to local.
...
```

#### <a name="apidoc.element.scp2.Client.prototype.write"></a>[function <span class="apidocSignatureSpan">scp2.Client.prototype.</span>write (options, callback)](#apidoc.element.scp2.Client.prototype.write)
- description and source-code
```javascript
write = function (options, callback) {
  var destination = options.destination;
  destination = unixy(destination);

  var attrs = options.attrs;
  var content = options.content;
  var chunkSize = options.chunkSize || 32768;

  var self = this;

  this.sftp(function(err, sftp) {
    if (err) {
      return callback(err);
    }

    var _write = function(handle) {
      self.emit('write', options);
      var length;
      var lastIndex = 0;
      var lastCursor = 0;

      if (Buffer.isBuffer(content)) {
        var contents = [];
        length = parseInt((content.length - 1) / chunkSize, 10) + 1;

        for (var i = 0 ; i < length; i++) {
          contents.push(content.slice(i * chunkSize, (i + 1) * chunkSize));
        }
        async.eachSeries(contents, function(buf, callback) {
          self.emit('transfer', buf, lastCursor, length);
          sftp.write(handle, buf, 0, buf.length, lastIndex, function(err) {
            lastIndex += buf.length;
            lastCursor += 1;
            callback(err);
          });
        }, function(err) {
          sftp.close(handle, callback);
        });
      } else if (typeof content === 'number') {
        // content is a file descriptor
        length = parseInt((attrs.size - 1) / chunkSize, 10) + 1;
        var range = new Array(length);
        async.eachSeries(range, function(pos, callback) {
          chunkSize = Math.min(chunkSize, attrs.size - lastIndex);
          if (!chunkSize) {
            callback(err);
            return;
          }
          var buf = new Buffer(chunkSize);
          fs.read(content, buf, 0, chunkSize, lastIndex, function(err, byteRead, buf) {
            self.emit('transfer', buf, lastCursor, length);
            sftp.write(handle, buf, 0, buf.length, lastIndex, function(err) {
              lastIndex += buf.length;
              lastCursor += 1;
              callback(err);
            });
          });
        }, function(err) {
          sftp.close(handle, function(err) {
            fs.close(content, callback);
          });
        });
      } else {
        throw new Error('Content should be buffer or file descriptor');
      }
    };

    sftp.open(destination, 'w', attrs, function(err, handle) {
      if (err) {
        // destination is directory
        destination = path.join(
          destination, path.basename(options.source)
        );
        destination = unixy(destination);

        // for emit write event
        options.destination = destination;
        sftp.open(destination, 'w', attrs, function(err, handle) {
          _write(handle);
        });
      } else {
        _write(handle);
      }
    });
  });
}
```
- example usage
```shell
...
Make a directory on the remote server. It behaves like 'mdkir -p'.

- **write** 'function(options, callback) -> callback(err)'

Write content on the remote server.

'''js
client.write({
    destination: '/home/admin/data/file.txt',
    content: 'hello world'
}, callback)
'''

The options can contain:
...
```



# <a name="apidoc.module.scp2.client"></a>[module scp2.client](#apidoc.module.scp2.client)

#### <a name="apidoc.element.scp2.client.Client"></a>[function <span class="apidocSignatureSpan">scp2.client.</span>Client (options)](#apidoc.element.scp2.client.Client)
- description and source-code
```javascript
function Client(options) {
  this._options = options || {};

  this.remote = {};
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
