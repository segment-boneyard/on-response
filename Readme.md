# on-response

    Call back when a response is delivered.

## Example

```js
var onResponse = require('on-response');

app.use(function (req, res, next) {
    onResponse(req, res, function (err, summary) {
        var time = summary.response.time;
        console.log('X-Response-Time: ' + time + ' ms.');
    });
    next();
});
```

## API

### onResponse(req, res, callback)

    Call back when the response is delivered.