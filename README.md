# pushstate-https-server

[![License](https://img.shields.io/cocoapods/l/ReactNativeAutoUpdater.svg?style=flat)](https://spdx.org/licenses/MIT)

A simple static http/https file server that works with HTML5 Pushstate.

Defaults all routes to `index.html` in the given root directory. Treats all other files to be static, and routes urls with the given static directories to make them relative to root.

For example,

* `localhost` or `localhost/a/pushstate/route` will always return `index.html`.

* `localhost/assets/emoji.png` or `localhost/a/pushstate/route/assets/emoji.png` will always return `assets/emoji.png` when `assets` directory is given as one of the static directories.



### Install

`npm install git+ssh://github.com/williamle8300/pushstate-https-server.git --save`

### Usage

```shell
$ pushstate-https-server -r rootDir -p 8000 -s -c certFile -k keyFile -d assets,styles,scripts
```

