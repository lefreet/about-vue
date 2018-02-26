# 开发环境

## 网络

> 每个程序员都应该有把梯子

* 推荐：[一枝红杏](https://www.hongxingwangzhi.com/)

要求能正常访问:
  - [google](https://www.google.com/)
  - [github](https://github.com/)
  - [npm](https://www.npmjs.com/) 
  - [stackoverflow](https://stackoverflow.com/)

---

## 用nvm管理node版本(可选)

> Node Version Manager <br>
> 需要经常变更node版本的情况，请先卸载原有nodejs，再安装nvm

#### 1. 安装

* 不需要安装nvm的，[点击这里](http://nodejs.cn/download/)直接下载安装`nodejs`
* windows系统下安装[nvm-windows](https://github.com/coreybutler/nvm-windows)，[点击这里](https://github.com/coreybutler/nvm-windows/releases)下载`nvm-setup.zip`，建议以管理员身份安装运行，安装后重启命令行窗口。
* osx系统安装[nvm](https://github.com/creationix/nvm)，[点击](https://github.com/creationix/nvm)查看安装说明

#### 2. 下载镜像配置

* windows
```bash
nvm node_mirror https://npm.taobao.org/mirrors/node/
nvm npm_mirror https://npm.taobao.org/mirrors/npm/
```
* osx
```bash
export NVM_NODEJS_ORG_MIRROR=https://npm.taobao.org/mirrors/node
```

#### 3. 使用示例

```bash
# 先安装个旧版，比如spm依赖的0.10.0
nvm install 0.10.0
# 再装个最新稳定版，具体版本请看官网
nvm install 8.9.4 
# 切换nvm版本
nvm use 9.9.4
```

---

## npm的配置

> 对npm不了解的，可以先阅读[官网介绍 01 - 10小节](https://docs.npmjs.com/getting-started/what-is-npm)

#### 1. 用nrm管理npm包源

```bash
# 安装
npm install nrm -g

# 查看可用地址
nrm ls

# 切换到淘宝镜像
nrm use taobao

# 添加公司内部搭建的私有包源，取名strong
nrm add strong http://115.29.205.204:10001/

# 切换
nrm use strong
```

#### 2. `node-gyp`下载镜像配置

> node-gyp是node跨平台编译工具，不同系统下这里比较容易出现问题，报错内容包含node-gyp等字眼。有遇到问题大家多反馈，我再收集整理解决方案。ps: 大部分原因都是墙导致的

```bash
npm config set disturl https://npm.taobao.org/dist
```

## 必备工具

* 编辑器：推荐[Sublime Text](https://www.sublimetext.com/)或[VS Code](https://code.visualstudio.com/)，轻量好用
* vue调试工具：chrome商店搜索`Vue.js devtools`，辅助开发
* 翻译：chrome商店搜索`有道词典`，启用划词翻译
* 欢迎补充

---
