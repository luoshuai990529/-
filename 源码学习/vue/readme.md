vue2基础实现：https://github.com/luoshuai990529/Vue_realization



....未完待续 日后完善😢

**如何学习/调试Vue源码**：

1. 在Github中找到Vue对应代码仓库，找到稳定版本tag 比如vue3.2.xx
2. 安装Vue源码相关依赖：`npm/yarn install`
3. 执行打包操作`npm/yarn dev` 执行前修改脚本(添加**`--sourcemap`**)：
   `"dev": "node scripts/dev.js --sourcemap"`
   加这个是为了查看调试源代码时找到打包前源代码文件的代码映射,这样打包之后会生成一个`.map`文件
4. 通过packages/vue/dist/vue.global.js 调试代码
5. 新建html页面，引入vue.global.js文件即可debuger调试代码