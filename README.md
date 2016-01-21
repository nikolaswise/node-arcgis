# node-arcgis

[![npm][npm-image]][npm-url]
[![travis][travis-image]][travis-url]

[npm-image]: https://img.shields.io/npm/v/node-arcgis.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/arcgis
[travis-image]: https://img.shields.io/travis/esripdx/node-arcgis.svg?style=flat-square
[travis-url]: https://travis-ci.org/esripdx/node-arcgis

Node/Browser Javascript library for ArcGIS

## Install

```
npm install arcgis
```

## Usage

```js
var ArcGIS = require('arcgis')
var ago = ArcGIS(token)
```

## Contributing

[Open-2](CONTRIBUTING.md)

## License

[ISC](LICENSE.md)


## Project Goals

This project should be more than just a wrapper around our current REST API, but an aspirational and forward looking attempt to create what the REST API _could_ be. Some of the primary targets are below:

### Simple Simple Simple

The end goal is for everything to be as simple as possible. Simple code, simple structures, simple responses, simple docs. If things get complicated we're doing something wrong.

### Modular

Every method and function should be it's own self sufficient deal - both for ease of comprehension (one file does one thing) but also for consumption. Ideally, each module could be required independently and work great. This means we're using ES6!

### Promises

Practically all of these methods require making calls to ArcGIS servers. Since we can't control the time required to receive a response, most everything is Async and returns a promise.

### Value Added

This project should work to simplify and unify the conceptual model for the ease of the programmer. This library is a UI in the most basic sense of the term — we're providing an interface between the developer and the API, and that interface needs to be well designed and thought through to make the process and smooth, intuitive, and pleasurable as possible.

For example, getting an org's name, description, and summary is 2 calls to the REST API. In this library, that should be one call.

### Universal Iso-PolyMetric Server Client JS

This should run in node land on the server and in the browser as well. The same code should work the same way in both places. This will expand out to cover instances of on-premise server as well as ArcGIS Online.

### Revolutionary Framework: Vanilla JS

This is framework agnostic. No dependencies, should work anywhere and everywhere. No dojo, no angular, no jquery, no lodash, no nothin'.
