# tern-qunit

[![Build Status](https://secure.travis-ci.org/angelozerr/tern-qunit.png)](http://travis-ci.org/angelozerr/tern-qunit)
[![NPM version](https://img.shields.io/npm/v/tern-qunit.svg)](https://www.npmjs.org/package/tern-jqunit)

[tern-qunit](https://github.com/angelozerr/tern-qunit) is a plugin which adds support for [qunit.js](http://qunitjs.com/) to the JavaSript code intelligence system [Tern](http://ternjs.net/).

[tern-qunit](https://github.com/angelozerr/tern-qunit) provides :

 * the tern qunit plugin [qunit.js](https://github.com/angelozerr/tern-qunit/blob/master/qunit.js)

## Demo

You can play with [online demo](http://demo-angelozerr.rhcloud.com/CodeMirror-Java/qunit.html) which uses CodeMirror ((inside Web Browser).

You can see demos in this git project with CodeMirror in  [demos/qunit.html](https://github.com/angelozerr/tern-qunit/blob/master/demos/qunit.html) :

Here a screenshot with completion with CodeMirror QUnit completion :
 
![CodeMirror & Tern Qunit](https://github.com/angelozerr/tern-qunit/wiki/images/TernQUnitWithCodeMirror.png)

Here a screenshot with completion with Eclipse IDE QUnit completion :

![Eclipse & Tern QUnit](https://github.com/angelozerr/tern-qunit/wiki/images/TernQUnitWithEclipse.png)

If you wish to use Eclipse as IDE, see Eclipse support for [QUnit](https://github.com/angelozerr/tern.java/wiki/Tern-&-QUnit-support).

## Installation

tern-qunit works with the NodeJS [Tern Server][tern-server], and within a browser.

The easiest way to install tern-qunit is to use a recent version of
[npm][npm]. In the directory where you installed the [tern package][tern-npm],
simply run

```
$ npm install tern-qunit
```

## Configuration

`qunit` support QUnit.

### With Node.js

In order for Tern to load the tern-qunit plugin once it is installed, you must
include `qunit` in the `plugins` section of your [Tern configuration
file][tern-config].

Here is a minimal example `.tern-project` configuration file:

```json
{
  "libs":["ecma5"],
  "plugins": {
    "qunit": {}
  }
}
```

### With WebBrowser (CodeMirror)

See [demos/qunit.html](https://github.com/angelozerr/tern-qunit/blob/master/demos/qunit.html)

## Structure

The basic structure of the project is given in the following way:

* `qunit.js` the tern plugin.
* `demos/` demos with QUnit tern plugin which use CodeMirror.
* `test` test of the tern plugin.
