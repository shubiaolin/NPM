/************************************************************
*   执行nodejs 某些不知支持es6语法
*/
1.支持import 和 export 需引入 es6=》es5 的转换
"@babel/cli": "^7.8.4",
"@babel/core": "^7.8.7",
"@babel/preset-env": "^7.8.7",
"@babel/register": "^7.8.6",

2.加入 .babelrc 内容 {
                        "presets": [
                         "@babel/env"
                        ]
                    }

3.run configuration 的 node parameters 加入 -r @babel/register


/************************************************************
* nodejs 支持执行 ts
*/
1.引入
"ts-node": "^8.6.2",
"typescript": "^3.8.3"
2.run configuration 的 node parameters 加入 --require ts-node/register

