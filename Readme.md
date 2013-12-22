# on-response

  Call back when a request is finished.

## Example

```js
var onResponse = require('on-response');

app.use(function (req, res, next) {
  var start = Date.now();
  onResponse(req, res, function (err) {
    var duration = Date.now() - start;
    console.log('request duration: ' + duration);
  });
  next();
});
```

## API

### onResponse(req, res, callback)

  Call back when the request is finished.

## License

```
WWWWWW||WWWWWW
 W W W||W W W
      ||
    ( OO )__________
     /  |           \
    /o o|    MIT     \
    \___/||_||__||_|| *
         || ||  || ||
        _||_|| _||_||
       (__|__|(__|__|
```