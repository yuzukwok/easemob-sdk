# easemob-sdk

[![build status][travis-image]][travis-url]
[![Coverage Status][coveralls-image]][coveralls-url]
[![gitter][gitter-image]][gitter-url]
[![Dependency Status][DependencyStatus-image]][DependencyStatus-url]

[travis-image]: https://travis-ci.org/leoliew/easemob-sdk.svg?branch=master
[travis-url]: https://travis-ci.org/leoliew/easemob-sdk
[coveralls-image]: https://coveralls.io/repos/leoliew/TechChat/badge.svg?branch=master
[coveralls-url]: https://coveralls.io/r/leoliew/easemob-sdk
[gitter-image]: https://badges.gitter.im/Join%20Chat.svg
[gitter-url]: https://gitter.im/leoliew/TechChat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
[DependencyStatus-image]: https://gemnasium.com/leoliew/TechChat.svg
[DependencyStatus-url]:https://gemnasium.com/leoliew/TechChat

easemob nodejs sdk


## Installation

node:

```
$ npm install easemob-sdk
```

## Running node tests

Install dependencies:

```shell
$ npm install
```
Run em!

```shell
$ npm test
```

## Usage


```js
var easemob_sdk = require('easemob-sdk');
easemob_sdk.init(org_name,app_name,client_id,client_secret);
easemob_sdk.user.create( 'leo', 'leo_password', function(err, res, body) {
  if(err || (res.statusCode != 200)) {
    // Handle the error
  }
  else {
    //Handle the result
    var result = body;
  }
});

```
