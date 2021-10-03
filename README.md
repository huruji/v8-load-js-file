# v8-load-js-file

v8 嵌入js 应用中并实现模块化加载 js 文件的例子(commonjs)

> app.js

```js
const test = require('test/test.js')

log(test.a)
log(test.add(2,3))
```

> test.js

```js
function add (a, b) {
    return a + b;
}
module.exports = {
    a: test,
    add,
}
```

运行

```bash
./demo test/app.js
```


