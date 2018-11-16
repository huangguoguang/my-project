# my-project

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


1.单文件组件
    1.三个部分组成
        1.template
            只能存在一个根元素
        2.script
        3.style
            scoped:样式只在当前组件内生效
    2.子父级组件交互(通信)
        父->子 props
            数据传递类型限制
            数据类型验证
            多数据类型
            必选项
            默认值 
            obj.arr数据类型的默认值 
        子->父：emit  Event
    3.插槽
        单个插槽
        具名插槽
        作用域插槽：数据是子传父
        2.5.0之前要用template
    4.动态组件
        keep-alive