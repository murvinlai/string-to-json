string-to-json
==============

Convert a string representation of dot-notion key into json format object.
It is particularly useful for converting req.query with dot notation as the key into json.
e.g. a http query like this: canada.bc.yvr.name=Vancouver&canada.bc.yvr.id=1234&usa.ny.nyc.name=New%20York
or a req.query like this: req.query = { "canada.bc.yvr.name":"Vancouver", "canada.bc.yvr.id":1234, "usa.ny.nyc.name"="New%20York" }
will result in: {"canada":{"bc":{"yvr":{"name":"Vancouver","id":"1234"}}},"usa":{"ny":{"nyc":{"name":"New York"}}}}


-------------


## Purpose


## Installation
    $ npm install string-to-json

## Quick Start

```js
    var str2json = require('string-to-json');
    
    str2json.convert({"abc.def.g":2});

```


