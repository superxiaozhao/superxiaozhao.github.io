---
title: webpack配置
date: 2021-02-18 18:11:26
tags: 2021
categories: webpack
---

## webpack 配置

1.  全局安装webpack

   ```shell
   npm install webpack@3.6.0 -g
   
   ```
```
   

2.非全局安装webpack

     ```shell
npm install webpack@3.6.0
```

3.webpack.config.js

```js
const path = require('path')//node自带包
module.exports = {
    entry:'./src/main.js',
    output:{
        path:path.resolve(__dirname,'dist'),//动态获取路径
        filename:'bundle.js',
    },
}
```

4.package.json

```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "webpack"
  },
```

5.结论

如此下来webpack命令直接映射到npm上只需要npm run build 就相当于 执行webpack命令了



   