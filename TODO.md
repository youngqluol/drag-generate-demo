#### 组件配置部分：
一、功能：
1. 配置项动态渲染，数据部分与vuex中相应组件数据双向绑定

二、bugs
1. 组件宽高初始值

#### node服务
1. 配置koa跨域
1. 前端单独目录client



### issues
1. `vue-config.js`配置的devServer.proxy后，无法代理请求到本地服务器
- 原因：node版本问题
- 解决：1. node版本降级至12.16.1或以下 2. 尝试使用koa-cors中间件解决跨域问题？

2. 下载less-loader后，报错`TypeError: this.getOptions is not a function`
- 原因：less-loader版本过高。8.0版本后的配置方式跟之前不一样
- 解决：1.下载less-loader@6.0.0  2. 重新配置