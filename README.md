# promisifyhttprequest
Using bluebird to promisify Node's http.request

## Example code

```js
var request = require('promisifyhttprequest');

var myRequest = request({
    method: 'GET',
    protocol: 'https'
    host: 'nodejs.org',
    port: 80,
    path: '/api/http.html#http_http_request_options_callback',
}).then(function(value) {
    console.log('value:', value);
});
```