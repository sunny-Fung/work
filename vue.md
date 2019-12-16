# vue 开发的百家精华

## 报错提示

1. cannot read property 'xx' of undefined

```js
import path from "ramda/src/path";
console.log(path(["a", "b", "c"], data)); // 解决 cannot read property 'xx' of undefined
console.log(data.a && data.a.b && data.a.b.c);
```

2. 解决数字 0 问题

```js
import defaultTo from "ramda/src/defaultTo";
console.log(defaultTo("default_value", data)); // 解决数字 0 问题
console.log(data || "default_value");
```
