# 翼龙面板中文汉化 来自 [VLssu.com](https://vlssu.com/)

- 目前支持 翼龙面板 V1.8.1 （实际比此版本更高）；
- 汉化已完成至 用户面板 管理面板正在进行汉化 详情见汉化仓库 Projects ；
- 仅修改内核语言部分！您大可放心使用，我本人也在使用我的 Fork 版本 ；

## 注意事项
- 建议使用 **翼龙面板前端 V1.8.1** 进行汉化操作

- 不建议使用汉化仓库中的源码进行安装操作，汉化仓库源码仅适用于汉化操作！

- 不建议在安装第三方插件后进行汉化操作

- 不建议在翼龙官方仓库提交关于汉化问题的 issues

- 欢迎对我发起关于汉化不准确等问题的 issues

- 你可以自由使用我汉化修改后的软件，甚至删除位于 Panel 底部的署名

- 请尊重社区开发组的劳动成果，请勿违反翼龙面板前端的开源协议

- 我接受且仅接受关于汉化的问题，有关翼龙面板的使用等问题勿扰。（可付费打扰 XD）





## 如何进行汉化

### 访问汉化仓库
                
----
https://github.com/vlssu/panel

### 下载源码并进行覆盖操作
                
----
下载源码 将 `resources` 与 `app` 文件夹对安装后的面板文件进行覆盖操作

PS：你也可以直接`clone`本项目，因为我是基于最新发布的版本进行汉化的，只替换这两个是不够的，你需要将`package.json` `yarn.lock`也替换一下，因为部分依赖原因。。。


### 重新构建面板
                
----
> 此部分引用于 https://pterodactyl.io/community/customization/panel.html
> Panel 的前端是用 React 构建的。 对源文件的任何更改都需要重新编译。
以下部分说明了如何执行此操作。 

##### 1.安装依赖项
`以下命令将安装构建面板所需的依赖项。 构建工具需要 NodeJS，yarn 用作包管理器。`
```
# Ubuntu/Debian 系统
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
apt install -y nodejs

# CentOS 系统
curl -sL https://rpm.nodesource.com/setup_14.x | sudo -E bash -
sudo yum install -y nodejs yarn      # CentOS 7 系统
sudo dnf install -y nodejs yarn      # CentOS 8 系统
```
`接下来安装所需的 javascript 包`
```
npm i -g yarn      # 安装yarn

cd /var/www/pterodactyl  #进入面板前端目录，请按您的运行环境进行调整
yarn       # 安装面板构建依赖项
```
##### 2.开始构建面板
`以下命令将重新构建 翼龙面板前端。`
```
cd /var/www/pterodactyl     #进入面板前端目录，请按您的运行环境进行调整
yarn build:production       # 开始构建面板
```

`您可以使用命令 yarn run watch 几乎实时地查看构建的进度`

> 本汉化部分文本基于[ilworkcn](https://github.com/ilworkcn) （由于该作者很长时间没去汉化最新的了，所以我自己汉化了一手，毕竟有现成的为啥不去引用一波呢）
> 由于仓库不能直接fork他的，必须用官方的才能汉化最新的，所以我只(也只能)引用他部分有限的汉化文本，而不是直接完全复制粘贴哦~
