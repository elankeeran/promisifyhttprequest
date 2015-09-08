# promisifyhttprequest
Using bluebird to promisify Node's http.request

## Example code

```js
var request = require('promisifyhttprequest');

var myRequest = request({
    method: 'GET',
    host: 'nodejs.org',
    port: 80,
    path: '/api',
}).then(function(value) {
    console.log('value:', value);
});
```
