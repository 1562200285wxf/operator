# 用户登录组件
编号：cc_80_0006_login

## 功能描述
用于登录功能的前端界面，包括账号、密码的输入.

作者：王孝峰

## 使用方法
在该组件中另引用验证码组件，一同注册。
main.js中
1 先引入
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';
import identify from  './views/utils/identify.vue'
import cc_80_0006_login from  './views/login/cc_80_0006_login.vue'
2导出组件
Vue.component('identify',identify);
Vue.component('cc_80_0006_login',cc_80_0006_login);
3引入和应用组件
Vue.use(identify);
Vue.use(ElementUI);

## 注意事项
1 可能在组件中会存在相互调用的情况。
2 一定注意引入的地址
3 只要完成全局注册，test文件位置任意移动，进行测试。

## 使用
在测试界面中直接使用该组件
<template>
    <div>
        <cc_80_0006_login></cc_80_0006_login>
    </div>
</template>
即可

## 修改
验证码的大小直接在组件identify中
          contentWidth和contentHeight修改即可

