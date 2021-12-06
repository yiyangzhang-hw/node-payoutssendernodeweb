### Overview

This is a dependency for using and configuring [servicecore](https://github.paypal.com/NodeInfra/node-servicecore) for _payoutssendernodeweb_.

### Installation

Set your npm registry then install the package.

```
npm set registry http://npm.paypal.com/
npm install --save @paypalcorp/payoutssendernodeweb
```

### Usage

Create a [servicecore](https://github.paypal.com/NodeInfra/node-servicecore) client for this service and make a request.

```javascript
var servicecore = require('servicecore');

var client = servicecore.create('@paypalcorp/payoutssendernodeweb');

// example (replace this with an example specific to your service)
client.request(
    req, //Request Object
    {
        method: 'GET',
        path: '/v1/some/path',
        qs: {
            foo: 'bar',
            baz: 'boz'
        }
    },
    function (error, response) {
        console.log(response.body);
    });
```
