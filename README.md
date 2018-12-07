## vue迁移之路

*** 
* [1.0]
* [2.0](https://github.com/RLwu/vue-spider/tree/master/vue-cli-2.0)
* [3.0](https://github.com/RLwu/vue-spider/tree/master/vue-cli-3.0)
***

## 关于node版本的问题

### nvm，node，npm之间关系

* ```nvm```：nodejs 版本管理工具
* ```nodejs```：在项目开发时的所需要的代码库
* ```npm```：nodejs 包管理工具，管理 nodejs 的第三方插件

### 安装 nvm

```
安装命令：
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash

or Wget:
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
```

> 如果在新的终端输入 nvm 时提示：command not found: nvm，有可能是以下原因之一：

* 你的系统可能缺少一个 .bash_profile 文件，你可以创建一个此文件（可通过vi或vim命令），打开复制粘贴以下代码（安装nvm成功后终端的最好3行代码）进去，保存，然后再次运行安装命令；

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

* 你可能需要重新打开一个 terminal 窗口或标签页

如果上面没有解决问题，打开你的 .bash_profile 文件，并添加以下代码：
source ~/.bashrc

### nvm 常用命令

```
* nvm --help                          显示所有信息
* nvm --version                       显示当前安装的nvm版本
* nvm install stable                  安装最新稳定版 node 
* nvm install <version>               安装指定的版本，如果不存在.nvmrc,就从指定的资源下载安装 
* nvm uninstall <version>             删除已安装的指定版本，语法与install类似
* nvm use <version>                   切换使用指定的版本node 
* nvm ls                              列出所有安装的版本
* nvm ls-remote                       安装指定的版本，如果不存在.nvmrc,就从指定的资源下载安装 
* nvm current                         显示当前的版本
* nvm alias <name> <version>          给不同的版本号添加别名
* nvm unalias <name>                  删除已定义的别名
* nvm reinstall-packages <version>    在当前版本 node 环境下，重新全局安装指定版本号的 npm 包
```
