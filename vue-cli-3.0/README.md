# vue-cli-3.0

> A Vue.js project

## Build Setup

``` bash
# 安装新包
npm install -g @vue/cli
# OR
yarn global add @vue/cli

# 检查其版本是否正确 (3.x)
vue --version

# 创建项目
vue create name

# 通过 vue ui 命令以图形化界面创建和管理项目
vue ui

# Vue CLI 3 和旧版使用了相同的 vue 命令，所以 Vue CLI 2 (vue-cli) 被覆盖了。如果你仍然需要使用旧版本的 vue init 功能，你可以全局安装一个桥接工具：
npm install -g @vue/cli-init
# `vue init` 的运行效果将会跟 `vue-cli@2.x` 相同
vue init webpack my-project

# 在现有的项目中安装插件
vue add @vue/eslint
vue add router
vue add vuex

……

```