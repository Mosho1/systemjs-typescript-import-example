# systemjs-typescript-import-example

https://github.com/systemjs/systemjs/issues/1251

`jspm i`, Serve `index.html` and look at `app.js!transpiled`.

The `lodash/flow` module's source:

```
var createFlow = require('./_createFlow');
var flow = createFlow();
module.exports = flow;
```

is imported as `{default: [Function]}` in System but `[Function]` in node.
