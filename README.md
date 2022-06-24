# 翼龙面板中文汉化 来自 [VLssu.com](https://vlssu.com/)

- **本汉化基于源仓库实时汉化(即开发板)，可能与正式版内容对应不上。**
- 汉化已完成 详情见汉化仓库 Projects ；
- 仅修改内核语言部分！您大可放心使用，我本人也在使用我的 Fork 版本 ；

## 汉化作者说明
- 本汉化主要基于 [ilworkcn](https://github.com/ilworkcn) ，引用时间为2022年6月8日，此后 [ilworkcn](https://github.com/ilworkcn) 汉化部分我将不在引用，后续汉化或修改基于 [vlssu](https://github.com/vlssu) ，于 [ilworkcn](https://github.com/ilworkcn) 此后汉化没有任何关系 ~~(主要是从头汉化太头疼了，所以以[ilworkcn](https://github.com/ilworkcn)为基础上完善汉化)~~

- 当然，我使用面板会更频繁，所以我会第一时间知道我的面板哪边需要改进，因此，我汉化更改了以下部分
  - 将gravatar更换为cravatar （由于国内无法正常使用，所以我换了）

## 注意事项

- 不建议在安装第三方插件后进行汉化操作

- 不建议在翼龙官方仓库提交关于汉化问题的 issues

- 欢迎对我发起关于汉化不准确等问题的 issues

- 你可以自由使用我汉化修改后的软件，甚至删除位于 Panel 底部的署名

- 请尊重社区开发组的劳动成果，请勿违反翼龙面板前端的开源协议

- 我接受且仅接受关于汉化的问题，有关翼龙面板的使用等问题勿扰。（可付费打扰 XD）


## 如何进行汉化

### 访问汉化仓库
                
----
https://github.com/vlssu/panel-chinese

### 下载源码并进行覆盖操作
                
----
下载源码 将 `resources` 与 `app` 文件夹 `package.json` `yarn.lock` 文件 对安装后的面板文件进行覆盖操作

PS：你也可以直接`clone`本项目，因为我是基于最新发布的版本进行汉化的，所以你直接将我的覆盖你原本的程序会更好一点。（是的，我就是这样）


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

## 最后作者(vlssu)的话
- 有的人可能会很好奇，为什么要引用 [ilworkcn](https://github.com/ilworkcn) 的呢，他不是一直在汉化吗？
- 是的，他确实一直在汉化，但我想给我自己的面板更新的时候他停更许久也多处未汉化，导致我想汉化后给自己用，但就在2022年6月22日我才发现他又开始更新了，并且部署方式更加完善。
- 但我本人喜欢开发板（因为能第一时间体验到最新版本）所以我依旧对我的仓库进行汉化。
