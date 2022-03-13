<img align="right" width="240" src="https://cdn.jsdelivr.net/gh/ChirmyRam/ChirmyRam-OneDrive-Repository/odlogo.png">

# 🛖 七米蓝的仓库


> 不只分享资源，还分享经验。本站用作学习交流，不得用于任何商业活动推广盈利。本仓库永久链接发布地址：[ChirmyRam-OneDrive-Repository](https://github.com/ChirmyRam/ChirmyRam-OneDrive-Repository) [![](https://img.shields.io/github/forks/ChirmyRam/ChirmyRam-OneDrive-Repository?style=social&label=star)](https://github.com/ChirmyRam/ChirmyRam-OneDrive-Repository) 

> 联系：[📧邮件](https://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=office@chirmyram.top)

## 🎤 一、仓库介绍

出于由来已久的囤积癖、白嫖怪的素养、收集剪辑素材的需求，我收集了这些资源，哗啦啦搬来一堆东西一本满足，但整理起来也是真的费劲。本着开放与共享的精神，我创建了此仓库。文件储存于国际版 OneDrive ，订阅类型为 Office365 E5 Developer，分享文件的同时也在刷API实现玄学免费续订，刷上瘾了属于是。除了域名和服务器，其他没怎么花钱，老白嫖怪了，当然所花的精力没法估量。

影视资源大多为内封字幕的 mkv 格式，为了方便浏览，以中文名称拼音首字母、常用英文名称首字母为顺序建立文件夹索引，并将内容联系程度紧密的作品归类在了一起，当然可能有多种翻译，找不到时试试换个名称。网站被频繁访问会触发 OneDrive 的 API 调用限制，若报错 `activityLimitReached` 请刷新或稍后再试。若下载太慢请使用高速的全局代理或多线程下载器。在 PC UA 模式下可查看文件（夹）大小。动画资源主要来自 [1ove论坛](https://www.qian.blue/archives/1ove-club.html) ，电子书、电影、电视剧资源主要来自阿里云盘各种资源分享渠道。批量搬运阿里云盘资源的教程请参阅 [自建阿里云盘webdav功能并搬运资源](https://www.chirmyram.top/archives/aliyunwebdav) 。为缩短本页版面，我对文字说明进行了折叠处理，点击每个标题下的 **▶【查看详情】** 展开完整内容。

## 🏷️ 二、标签介绍

<details>
  <summary>【查看详情】</summary>

### 1. 盘符介绍

不同的OneDrive目录程序所能挂载账户数量不尽相同，而我又不忍舍弃，所以部分网站同时挂载了六个盘，部分只挂载了一个盘。当然 **Root** 这个盘符是对网站整体六个盘抽象而言的，并不存在这样一个OneDrive账户。

- ![](https://img.shields.io/badge/Root-orange) 总盘 ：同时挂载以下六个盘。
- ![](https://img.shields.io/badge/Rep-orange) 仓库盘 ：存放杂七杂八的资源。
- ![](https://img.shields.io/badge/Ani-orange) 动画盘 ：存放动画资源。
- ![](https://img.shields.io/badge/Mov-orange) 电影盘 ：存放电影、纪录片资源。
- ![](https://img.shields.io/badge/Doc-orange) 图书盘 ：存放电子书资源。
- ![](https://img.shields.io/badge/Tlv1-orange) 剧集一盘 ：存放亚洲电视剧资源。
- ![](https://img.shields.io/badge/Tlv2-orange) 剧集二盘 ：存放欧美电视剧资源。

### 2. 标签介绍

绿色标签为**部署平台**，黑蓝标签为部署所用的**程序工具**，橙色标签为**挂载盘符**。可点击标签直接访问相关官网，程序软件均有部署教程。

以 [![](https://img.shields.io/badge/CFW-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/qkqpttgf/OneManager-cfworkerskv?style=flat&label=star)](https://github.com/qkqpttgf/OneManager-cfworkerskv) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://com.chirmyram.com/) 为例，意为在 **CFW** 上使用 **OneManager** 挂载了**六个盘**。

</details>

## 🛫 三、平台评测

<details>
  <summary>【查看详情】</summary>

首先引入两个概念：SaaS ， PaaS。
SaaS ，Software-as-a-Service ，意为软件即服务。平台为用户提供软件部署、托管服务，用户不必自己配置。
PaaS ，Platform as a Service ，意为平台即服务。平台为用户提供软件开发、运行环境等整套服务，侧重于开发。

这是我的浅薄理解，当然在这里也不必深入理解、甚至还会混为一谈，介绍它俩是为了方便在谷歌搜索相关内容，同义搜索词还有 free cloud container 、free cloud hosting 等等。只需要知道这些平台都有一个共同的特点：用户可以将程序项目放到云服务平台持续运行，平台已经预先提供了相应的运行环境。

为了方便这里就简称云平台了，以此来看，如[腾讯云函数](https://cloud.tencent.com/product/scf/)、 [heroku](https://www.heroku.com/) 已经是为众多折腾玩家所周知。部署方式多为从 github 仓库拉取源码、使用CLI命令行工具从本地上传源码等，大多为 docker 容器服务构建，即源码等东西放进去就没法修改或取不出来，不同于 VPS 具有完整的 Linux 环境，这些云平台的环境都是指定的，选则后除非删除否则无法自由更改。这类云平台在国内较少，就那几大云服务商的云函数，限制比较多，国外倒是多如牛毛，这里有一个别人总结的、为开发者提供一定免费额度服务的平台 [free-for-dev](https://github.com/ripienaar/free-for-dev) ，点进每个平台应直奔 Price 页面看价格套餐。薅羊毛必备，我上穷碧落下黄泉尝试了好几家，实在折腾得够呛。

|平台|性质|免费额度|主要限制|部署方式|自定义域名|
|----|----|----|----|----|----|
|[heroku](https://www.heroku.com/)|虚拟化容器服务|每月总计550小时、绑定信用卡达1000小时|超30分钟不活跃将休眠并重置数据、每24小时重启并重置数据|拉取 github 仓库、CLI 命令行工具|绑定信用卡才能自定义域名，否则自行反代、付费才能配置 https|
|[vercel](https://vercel.com/)|静态网页服务|每月总计100G流量|每天部署100次、部署的网站被访问过多会发邮件警告封号|拉取 github 仓库、CLI 命令行工具|通过 CNAME 解析自定义域名、自动生成 SSL 证书、自动重定向至 https|
|[glitch](https://glitch.com/)|静态网页服务|每月总计1000小时|超30分钟不活跃将休眠|拉取 github 仓库|通过 CNAME 解析自定义域名、自动生成 SSL 证书、自动重定向至 https|
|[netlify](https://www.netlify.com/)|静态网页服务|每月总计100G流量、每月总计构建300分钟、站点数量无限|只能同时构建1个实例|拉取 github 仓库、CLI 命令行工具|通过 CNAME 解析自定义域名、自动生成 SSL 证书、自动重定向至 https|
|[okteto](https://okteto.com/)|虚拟化容器服务|最大部署10个实例|每日重置数据、容易封号|拉取 github 仓库、docker 命令、CLI 命令行工具|免费版不支持，自行反代|
|[railway](https://railway.app/)|虚拟化容器服务|每月5美刀|需要使用注册已达30天的 github 账户来注册它、风控较严|拉取 github 仓库、CLI 命令行工具|通过 CNAME 解析自定义域名、自动生成 SSL 证书|
|[fly.io](https://fly.io/)|虚拟化容器服务|每月总计2340小时、160G流量|需绑定信用卡才能获得（不验证扣款）、各地区流量额度不同|CLI 命令行工具|通过 CNAME 解析自定义域名、自动生成 SSL 证书、不会重定向至 https|
|[render](https://render.com/)|虚拟化容器服务|静态网页每月100G流量、 Web 服务每月总计750小时|需绑定信用卡才能获得Web服务额度（会验证扣款）、 Web 服务超15分钟不活跃将休眠并重置数据、 Web 服务随时重置并丢失数据|拉取 github 仓库|通过 CNAME 解析自定义域名、自动生成 SSL 证书、自动重定向至 https|
|[koyeb](https://www.koyeb.com/)|虚拟化容器服务|2个实例|注册需要等待审核、实例会重启丢失数据|拉取 github 仓库、docker 命令、CLI 命令行工具|目前不支持，自行反代|
|[replit](https://replit.com/)|IDE 服务|500M储存空间、500M RAM、0.2 - 0.5 vCPUs|IDE 终端无 root 权限、实例不活跃将休眠|拉取 github 仓库、IDE 终端执行|通过 CNAME 解析自定义域名、自动生成 SSL 证书、自动重定向至 https|
|[goorm](https://ide.goorm.io/)|IDE 服务|5个实例|只能同时运行一个实例、实例不活跃将休眠|IDE 终端执行|免费版不支持，自行反代|
|[cloudflare](https://www.cloudflare.com/zh-cn/)|CDN 、域名、代码托管服务| CFW 请求10W次/天、 CFP 请求10W次/天|自定义域名必须更改域名 NS 至 cloudflare|CFW 为手动填写代码或从 github 仓库拉取、CFP 为从 github 仓库拉取代码|CFW 为配置路由规则并 CNAME 解析域名，可能需要配置页面规则实现自动重定向到 https 、CFP 为直接 CNAME 解析域名并直接重定向至 https|

解读：

- 简介：部分超过一定时间不活跃会休眠的容器平台，适合部署那些即搭即用的项目，比如代理节点、解析下载工具、静态网页服务等测试项目，否则再次唤醒丢失部署后的所有更改超级麻烦，一夜回到解放前。使用免费的云数据库平台可以有效解决重置数据的问题，前提是这些项目支持使用数据库而且数据量不能太大，如 MySQL 云数据库 [db4free](https://db4free.net/) 、PostgreSQL 云数据库 [ElephantSQL](https://www.elephantsql.com/) 、MongoDB 云数据库 [MongoDB](https://www.mongodb.com/) 。

- 虚拟化容器服务：非常容易丢数据，所谓丢数据也就是恢复到初始状态，期间的任何更改被还原，不适合拿来弄经常变动的东西，比如挂载 OneDrive 就需会经常刷新 refresh token 。那有什么不会经常变的东西呢？比如一些纯工具站，如我搭的 [m3u8 视频在线下载器](https://m3.chirmyram.com/) 、网站监控工具 [Uptime Kuma](https://up.chirmyram.com/) ，前者属于静态网页且工作时比较吃CPU，上表很多平台可以部署，后者为 JavaScript 程序，需要 nodejs 环境或使用 docker 部署，提前配置好，连同配置一起丢进去部署，任它再怎么重置也还能正常工作。

- [fly.io](https://fly.io/)  ：Dockerfile 兼容性较差，别家都能用的 Dockerfile 在它这里总是报错无法成功部署。目前就在上面搭了几个 [v2ray 节点](https://github.com/lyz7805/v2ray4flyio) ，无论怎么重置数据也还是能用。

- 信用卡：部分平台需要绑定国外信用卡才能获得或提升额度。如 [fly.io](https://fly.io/) 和 [render](https://render.com/) ，这俩可以用虚拟信用卡过审核，我使用的是[易贝卡](https://www.easypayx.com/card)，申请教程见[视频教程](https://youtu.be/hKib4CAMKYo)、[文字教程](https://bbs.1ove.club/thread-6070.htm)。但是过不了甲骨文、GCP、AWS等平台，它们风控极为严格。

- CFW 、 CFP ：即 Cloudflare Workers 、Cloudflare Pages，前者托管 javascript 网页，后者为托管静态网页。我也很看重自定义域名的方式、是否支持 https ，如你所见我的所有分站都是自己的域名且自动重定向到了 https 。我更喜欢通过 CNAME 解析来自定义域名，否则就用 CFW 反代、添加 CFW 路由规则来自定义域名。反代教程见 [Onedrive+OneManager+Heroku+CFWorkers免费的OD列表](https://www.wangfuchao.com/458/) ，只有一个站就把两个分流地址改成一样的。

- TOS ：网站底部或文档中的 Terms of Service ，即服务条款，各平台都会封禁搭建离线下载、群发垃圾邮件、色情暴力等服务，均属滥用范畴违反服务条款，而 [heroku](https://www.heroku.com/) 还会封禁梯子代理服务。提前排个雷，我已被这俩平台封了大小号（很多平台我注册了多个号都没事）：
[okteto](https://okteto.com/)：大号搭建 qBittorrent 下 bt ，倒是不冤，以身试法。不过这家封号真的喜怒无常，不只我有这种情况，我自认为小号搭的东西没有违反 TOS 也给封了。
[railway](https://railway.app/)：被封原因为注册多个账户，这个就很冤了，我就因为梯子速度太慢换了个节点多刷新了几次就给 ban 了。索性当场注册个小号也还是没了。

- 安卓：我的个别分站有 [![](https://img.shields.io/badge/Android-brightgreen?&style=flat)](https://f-droid.org/packages/com.termux/) 标签，这是我将退役的华为畅享 6 折腾成为服务器后搭建的，物尽其用榨干最后一滴价值，就不再列入表中了。装上软件 [Termux](https://f-droid.org/packages/com.termux/) ，在 [Termux](https://f-droid.org/packages/com.termux/) 里面装上精简 [Centos8](https://f-droid.org/zh_Hans/packages/exa.lnx.a/) 子系统，连环套娃，然后使用内网穿透的方式搭建网站，所以失联是家常便饭，稳定性随缘。我部署了很多具有试玩性质的项目，更多部署经验参阅 [将手机内网穿透当作服务器并运行了几个项目](https://www.chirmyram.top/archives/phoneserver) ，不过现在我网站备案掉了使用的是自建的 frp 穿透。

</details>

## 🔣 四、程序鉴赏

<details>
  <summary>【查看详情】</summary>

挑选目录程序，我首先考虑能否在云托管平台一键部署，再考虑在 VPS 上部署，如果云平台无法部署、VPS 部署麻烦，就只能舍弃了，还考虑是否支持自动刷新 refresh token ，token 有效期三个月，毕竟重新获取一次还是挺麻烦的。我尤其偏爱利用 Golang 编写的程序，单个二进制文件直接执行、nginx 反代、supervisor 实现后台运行并守护进程，一条龙直接带走，也不需要考虑运行环境、依赖库、版本问题。

|程序|语言|运行环境|多账户|搜索范围|WebDAV|美化程度|
|----|----|----|----|----|----|----|
|[alist](https://github.com/Xhofe/alist)|Golang|直接运行|✔|✖|网盘转 WebDAV （读写）、WebDAV 访客账号（只读）|自定义|
|OneManager（[PHP](https://github.com/qkqpttgf/OneManager-php)、[CFW](https://github.com/qkqpttgf/OneManager-cfworkerskv)）|PHP、JavaScript|PHP、CFW|✔|✖|✖|多主题|
|[OneIndex](https://github.com/motao123/oneindex)|PHP|PHP（composer ）|✖|✖|✖|多主题|
|[FODI](https://github.com/vcheckzen/FODI)|JavaScript，HTML|CFW，Web|✖|✖|✖|简约|
|[onedrive-vercel-index](https://github.com/spencerwooo/onedrive-vercel-index)|TypeScript|Vercel|✖|✖|✖|简约|
|[gonelist](https://github.com/gonelist/gonelist)|Golang|直接运行|✖|全盘|✖|简约|
|[sharelist](https://github.com/reruin/sharelist/tree/0.1)|JavaScript|nodejs|✔|✖|网盘转 WebDAV（只读）|简约|
|[zfile](https://github.com/zhaojun1998/zfile)|Java|Java|✔|✖|✖|简约|
|[OLAINDEX](https://github.com/WangNingkai/OLAINDEX)|PHP|PHP（composer ）|✔|当前目录|✖|多主题|
|[PanIndex](https://github.com/libsgh/PanIndex)|Golang|直接运行|✔|全盘|WebDAV 转目录|多主题|
|[onepoint](https://github.com/ukuq/onepoint)|JavaScript|nodejs、CFW|✔|✖|✖|简约|
|[YukiDrive](https://github.com/YukiCoco/YukiDrive)|C#|直接运行|✔|✖|✖|简约|
|[PyOne](https://github.com/abbeyokgo/PyOne)|Python|Python3、Redis、MongoDb（Aria2）|✔|✖|✖|简约|
|CuteOne（[Python](https://github.com/Hackxiaoya/CuteOne)、[PHP](https://github.com/Hackxiaoya/CuteOneP)）|Python、PHP|Python3, MySQL, MongoDb、PHP（composer ）|✔|全盘|✖|简约|
|[JustList](https://github.com/txperl/JustList)|Python|Python3|✔|全盘|✖|简约|
|[OneList](https://github.com/MoeClub/OneList)|Python、Golang|Python3、直接运行|✔|✖|✖|简约|
|[nextlist](https://github.com/lixiaofei123/nextlist)|Golang|直接运行，MySQL|✔|✖|✖|简约|

解读：

- 简介：此表根据我的偏好习惯总结而来，我体验过上面大部分程序，差不多摸清了性质。更多细节请仔细阅读程序作者的介绍。如部分程序支持多账户挂载，多账户不单指 OneDrive 账户，还有国内外其他网盘、对象储存空间、文件传输协议。美化程度中多主题指程序内置预设好的多个主题，其他选项意为无法切换主题或自己修改代码切换主题。

- 全盘搜索：OneDrive 本身提供的全盘搜索 API 极为拉跨，程序要实现全盘搜索，一般首先会检索 OneDrive 中所有文件，在搭建环境中生成索引数据库，少量文件体验当然极为顺畅，但对于储存了海量文件的 OneDrive 简直是灾难，检索一遍极其耗费时间、检索结果不全造成大量空目录、触发 OneDrive API 调用限制导致网站崩溃、文件更新后无法及时跟进。故弃用。而 [gonelist](https://github.com/gonelist/gonelist) 则搭在手机上试玩。

- 运行环境： CFW 指 cloudflare workers ，和运行环境 vercel 一样，都是专为这些云托管平台而设计，因此直接将平台当做运行环境。[PyOne](https://github.com/abbeyokgo/PyOne) 的运行环境中有 Aria2 ，是因为它支持离线下载到 OneDrive ，这是一个可选功能，按需安装。

- WebDAV ：表中所指的 WebDAV 有两种情况。网盘转 WebDAV（只读）：指将挂载好的网盘实现 WebDAV 功能，和支持 WebDAV 的软件对接来实现查看文件，目前均只支持文件只读模式，即只能看不能改，属于扩展功能，适合公开分享；WebDAV 转目录：指将其他网盘提供的 WebDAV 挂载为网页端文件列表，公开展示出来，这也是这些目录程序的初始作用。

- [alist](https://github.com/Xhofe/alist) ：可以使用免费的远程云数据库将其部署至 [heroku](https://www.heroku.com/) 或 [render](https://render.com/) ，参照项目 [alist-heroku](https://github.com/sbwml/alist-heroku) ，在应用休眠后再次唤醒不会丢失数据。需要注意的是：在 [heroku](https://www.heroku.com/) 上部署后使用应用默认的域名、 CFW 反代加速可正常使用 WebDAV 功能，而 CFW 反代之后又自定义域名会导致 WebDAV 功能失效无法连接；在 [render](https://render.com/) 上面部署后使用默认域名、自定义域名均无法使用 WebDAV 功能，测试发现 [render](https://render.com/) 的应用默认域名也使用的 Cloudflare 的CDN，猜测就是这个因素影响了 WebDAV。

- [OneIndex](https://github.com/motao123/oneindex) ：原仓库已被作者删除，我用的是众多魔改分支中的一个，看图模式来自[闲得没事做改了一下 oneindex 的看图模式](https://www.hostloc.com/thread-484078-1-1.html)，评论系统来自 [oneindex网盘添加gitalk评论系统](https://iwalyou.com/515.html) ，主题美化来自[自带主题 nexmoe 的美化修改](https://github.com/Zisbusy/OneIndex-theme)。除此之外还有其他较为有特色的魔改版：[oneindex-j](https://github.com/jialezi/oneindex-j) 支持挂载国际版 Sharepoint 、世纪互联 OneDrive 及 Sharepoint ， 但仍只支持挂载一个账户；[OneindexN](https://github.com/xieqifei/OneindexN) 支持全盘搜索、aria2 离线下载，全局搜索为onedrive官方返回的结果，搜索结果并不准确；[OneindexM](https://github.com/Mintimate/OneindexM) 在 [OneindexN](https://github.com/xieqifei/OneindexN) 的基础上进行了修复和优化。

- [FODI](https://github.com/vcheckzen/FODI) ：前后端分离，后端部署于 CFW ，前端部署于 CFP ，也可部署于其他静态网站云平台或 VPS 主机，初次加载较慢需要数秒，加载完毕后就像在本地浏览文件一样，体验相当丝滑。

- [sharelist](https://github.com/reruin/sharelist/tree/0.1) ：表中所列出的是0.1版本，非最新版，0.1存在较多致命 bug ，如挂载账户超过1个所有账户的路径都会指向同一个，使用 WebDAV 播放视频时间一长就会导致整个网站变为所播放视频视频的直链，相当令人头痛，曾尝试搭建分站来解决问题，同时运行多个 nodejs 进程也很不方便，迫于是当时发现唯一支持挂载网盘为 WebDAV 只读功能的程序，就一直用着，憋得慌。而新版目前仍在开发中，文档也不完善，而且新版的 bug 还是巨多。直到遇见 [alist](https://github.com/Xhofe/alist) ，完美的解决了问题，同时挂载多个盘也实现了 WebDAV 只读，立马弃用 [sharelist](https://github.com/reruin/sharelist/tree/0.1) 。

- [zfile](https://github.com/zhaojun1998/zfile) ：众所周知 Java 程序向来极为占用资源，放在 VPS 上有些奢侈了，所以我只是部署在了手机上试玩。功能确实强大，浏览体验也很顺畅。

</details>

## 🚀 五、批量搬运

<details>
  <summary>【查看详情】</summary>

> 使用原始的批量下载工具进行下载也行，不过更推荐认识一下 [Rclone](https://rclone.org/) 。

[Rclone](https://rclone.org/) 是一个支持多种云储存平台、国外云盘、储存协议的命令行工具，兼容 OneDrive 独特的 WebDAV 功能，自行搜索使用教程。在其他资源账户中，赋予域内另一空白账户对其资源文件夹的**只可查看权限**，即**只读权限**，使用 [Rclone](https://rclone.org/) 配置该空白账户及资源文件夹链接，自动加密账户密码，既可共享出来以供他人批量搬运资源，又能：限制操作权限、避免泄露密码、避免没有创建 API 权限的尴尬、不必担心 refresh token 过期。直接在 [Rclone](https://rclone.org/) 配置文件中填入下述配置，不必再逐步配置，再次配置会导致已被加密的密码再次被加密， [Rclone](https://rclone.org/) 无法识别真实密码从而报错。配置名 `[root]` 即为盘符名，配置名在 [Rclone](https://rclone.org/) 中称为 `remote` 。

[Rclone](https://rclone.org/) 还有相对简便易用的图形界面程序 [RcloneBrowser](https://github.com/kapitainsky/RcloneBrowser/releases) ，如果命令行用起来不太顺手可以试试。下载核心程序 [Rclone](https://rclone.org/downloads/) 解压，下载图形界面程序 [RcloneBrowser](https://github.com/kapitainsky/RcloneBrowser/releases)  安装。新建一个 `rclone.conf` 文本文件，将下述配置文件复制进去。在图形程序中，点击左上角 `file` → `preferences` ， `rclone location` 选择解压出的 rclone 核心主程序 `rclone.exe` ， `rclone.conf location` 选择新建的 `rclone.conf` 文件。回到图形程序界面点击左下角 `refresh` 刷新出配置，最后就可以浏览文件批量下载了，在顶部第二行 `Jobs` 中查看传输进程。

- [Rclone](https://rclone.org/) 配置文件

```
[root]
type = webdav
url = https://al.chirmyram.com/dav/
vendor = other
user = alist
pass = kCJQSyuVJDmwgI0BM60Mtum8VGnI
```
```
[rep]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/pub_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```
```
[ani]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/ani_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```
```
[mov]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/mov_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```
```
[doc]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/doc_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```
```
[tlv1]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/tlv_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```
```
[tlv2]
type = webdav
url = https://chirmyram-my.sharepoint.com/personal/tlv2_chirmyram_top/Documents/
vendor = sharepoint
user = croffice@chirmyram.top
pass = ia4QaFUxBYI8crnhR3m5wBbkDncmhSYt7oNBFg
```

这里有两种 WebDAV 服务，分为 [alist](https://github.com/Xhofe/alist) 自建和 OneDrive 官方。更多实现 OneDrive WebDAV 的方式请参考我的博客文章[让 OneDrive 实现 WebDAV 服务](https://www.chirmyram.top/archives/onedrivewebdav) 。

 [alist](https://github.com/Xhofe/alist) 挂载 OneDrive 的同时也能实现 WebDAV 服务来方便浏览文件，当然也可以将它放进支持 WebDAV 的文件管理器中进行批量搬运，也不会走自建服务器的流量，所以我把所有盘都挂上去了。 [alist](https://github.com/Xhofe/alist) 的 WebDAV 访客账号对文件只有**只读**权限，即只能读取无法操作，实属理想的公共 WebDAV 服务。但这只是我自建的 WebDAV 服务，远不如微软官方的稳定。

OneDrive 商业版本身不支持目前通行的 WebDAV 协议，但它确实有比较特殊的 WebDAV 功能。以我的 E5 OneDrive 登录后首页根目录地址为例：
```
https://chirmyram-my.sharepoint.com/personal/pub_chirmyram_top/_layouts/15/onedrive.aspx
```
则其对应的 WebDAV 链接为：
```
https://chirmyram-my.sharepoint.com/personal/pub_chirmyram_top/Documents/
```
观察其特点可发现，将末尾的 `/_layouts/15/onedrive.aspx` 替换为 `/Documents/` 就可以了。末尾 /Documents/ 即为 OneDrive 根目录，也可在其后继续添加子目录。

建议少量分批次搬运，否则我修改部分资源的时候会导致搬运任务出错，前功尽弃。两个网盘对拷不会占用本地储存空间，当然流量还是烧的自己的，而且是双倍流量，不过部分 VPS 商家不会计算进入VPS 的入网流量。还可以使用微软官方 OneDrive 搬运工具 [Mover](https://app.mover.io/) 在两个账号之间搬运资源，高速稳定，一天可搬1T（前提是得有两个账号的密码、单文件上限15G）。

</details>

## 🌟 六、特别推荐

<details>
  <summary>【查看详情】</summary>

酒香还怕巷子深，有部分资源初具规模但体积不够大（同类资源未超过5T），没有独立存放到一个盘上，而是杂七杂八散落在了仓库盘，不方便查找，于是在这里特别推荐。若链接无法访问请在第七章分站中按相同路径查找。

1. [欧路词典库](https://al.chirmyram.com/rep/Doc/%E6%AC%A7%E8%B7%AF%E8%AF%8D%E5%85%B8%E5%BA%93)

共25本英语词典，含离线语音文件，排版精美，与纸质版一致。

2. [音乐](https://al.chirmyram.com/rep/Music)

周杰伦全套 、许嵩全套、部分ACG音乐及其他杂七杂八我喜欢听的歌，能下到无损的均为无损，内嵌专辑封面、歌词。

3. [软件合集](https://al.chirmyram.com/rep/PC/sof)

包含由 [@vposy](https://weibo.com/u/1112829033) 修改的 Adobe 全家桶、 [NextITellYou](https://next.itellyou.cn/) 整站 Windows 官方镜像文件（截止2021-12-21）、[软件安装管家](https://mp.weixin.qq.com/s/3uYhgpRpkfo2hBNhuW-zpw)微信公众号软件目录整套软件（截止21年12月Win版），当然第一部分装机必备里面烂大街的软件没有搬。

</details>

## 📂 七、分站一览

> **✅/🔴  各分站状态实时监控：[https://up.chirmyram.com/](https://up.chirmyram.com/)**

### 1.总盘

- ▶ 1.1 [https://al.chirmyram.com/](https://al.chirmyram.com/) [![](https://img.shields.io/badge/TCT-brightgreen?&style=flat)](https://cloud.tencent.com/product/lighthouse) [![](https://img.shields.io/github/stars/Xhofe/alist?style=flat&label=star)](https://github.com/Xhofe/alist) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://al.chirmyram.com/)

**特别提示：** 网页在线播放器无法识别内封字幕、不兼容部分视频编码，需使用 WebDAV 播放器或下载到本地播放。 [alist](https://github.com/Xhofe/alist) 挂载 OneDrive 的同时也能实现 WebDAV 服务来方便浏览文件，当然也可以将它放进支持 WebDAV 的文件管理器中进行批量搬运，所以我把所有盘都挂上去了。 [alist](https://github.com/Xhofe/alist) 的 WebDAV 访客账号对文件只有**只读**权限，即只能读取无法操作，实属理想的公共 WebDAV 服务，所以我现在首推它。 PC 端多媒体播放器推荐 [Potplayer](https://potplayer.daum.net/?lang=zh_CN) ，安卓端多媒体播放器推荐 [Nplayer](https://al.chirmyram.com/rep/Android/%E8%B0%B7%E6%AD%8C%E5%95%86%E5%BA%97/nPlayer_1.7.7.7_191219.apk) ，可显示视频内封字幕、音乐内封歌词；安卓端音乐播放器推荐 [cloudbeats](https://al.chirmyram.com/rep/Android/%E8%B0%B7%E6%AD%8C%E5%95%86%E5%BA%97/CloudBeats_1.8.4.apk) ，可较快生成播放列表并串流播放，留下的缓存也极小；安卓端电子书阅读器推荐[静读天下](https://al.chirmyram.com/rep/Android/%E8%B0%B7%E6%AD%8C%E5%95%86%E5%BA%97/Moon_Reader_Pro-v7.0_build_700005-M.apk)，支持多种电子书格式。
- WebDAV 配置参数

|参数|值|
|----|----|
|链接 / URL|https://al.chirmyram.com/dav/|
|主机 / Host|al.chirmyram.com|
|路径 / Path|/dav/|
|协议 / HTTPS|SSL|
|端口 / Port|443|
|账号 / User|alist|
|密码 / Password|alist|

注意：除非相关项目适配浏览器网页端，否则浏览器本身是不支持 WebDAV 协议的。

- ▶ 1.2 [https://om.chirmyram.com/](https://om.chirmyram.com/) [![](https://img.shields.io/badge/Euserv-brightgreen?&style=flat)](https://euserv.com/) [![](https://img.shields.io/github/stars/qkqpttgf/OneManager-php?style=flat&label=star)](https://github.com/qkqpttgf/OneManager-php) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://om.chirmyram.com/)

- ▶ 1.3 [https://op.chirmyram.com/](https://op.chirmyram.com/) [![](https://img.shields.io/badge/Euserv-brightgreen?&style=flat)](https://euserv.com/) [![](https://img.shields.io/github/stars/ukuq/onepoint?style=flat&label=star)](https://github.com/ukuq/onepoint) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://op.chirmyram.com/)

- ▶ 1.4 [https://zf.chirmyram.top/](https://zf.chirmyram.top/) [![](https://img.shields.io/badge/Android-brightgreen?&style=flat)](https://f-droid.org/packages/com.termux/) [![](https://img.shields.io/github/stars/zhaojun1998/Zfile?style=flat&label=star)](https://github.com/zhaojun1998/Zfile) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://zf.chirmyram.top/)

- ▶ 1.5 [https://oli.chirmyram.top/](https://oli.chirmyram.top/) [![](https://img.shields.io/badge/Android-brightgreen?&style=flat)](https://f-droid.org/packages/com.termux/) [![](https://img.shields.io/github/stars/WangNingkai/OLAINDEX?style=flat&label=star)](https://github.com/WangNingkai/OLAINDEX) [![](https://img.shields.io/badge/Root-orange?&style=flat)](https://oli.chirmyram.top/)

### 2. 仓库盘

- ▶ 2.1 [https://oi.chirmyram.com/](https://oi.chirmyram.com/) [![](https://img.shields.io/badge/Euserv-brightgreen?&style=flat)](https://euserv.com/) [![](https://img.shields.io/github/stars/motao123/oneindex?style=flat&label=star)](https://github.com/motao123/oneindex) [![](https://img.shields.io/badge/Rep-orange?&style=flat)](https://oi.chirmyram.com/)

- ▶ 2.2 [https://cfdrep.chirmyram.com/](https://cfdrep.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Rep-orange?&style=flat)](https://cfdrep.chirmyram.com/)

- ▶ 2.3 [https://vcrep.chirmyram.com/](https://vcrep.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Rep-orange?&style=flat)](https://vcrep.chirmyram.com/)

- ▶ 2.4 [https://gl.chirmyram.top/](https://gl.chirmyram.top/) [![](https://img.shields.io/badge/Android-brightgreen?&style=flat)](https://f-droid.org/packages/com.termux/) [![](https://img.shields.io/github/stars/gonelist/gonelist?style=flat&label=star)](https://github.com/gonelist/gonelist) [![](https://img.shields.io/badge/Rep-orange?&style=flat)](https://gl.chirmyram.top/)

- ▶ 2.5 [https://oi.chirmyram.top/](https://oi.chirmyram.top/) [![](https://img.shields.io/badge/Android-brightgreen?&style=flat)](https://f-droid.org/packages/com.termux/) [![](https://img.shields.io/github/stars/motao123/oneindex?style=flat&label=star)](https://github.com/motao123/oneindex) [![](https://img.shields.io/badge/Rep-orange?&style=flat)](https://oi.chirmyram.top/)

### 3. 动画盘

- ▶ 3.1 [https://cfdani.chirmyram.com/](https://cfdani.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Ani-orange?&style=flat)](https://cfdani.chirmyram.com/)

- ▶ 3.2 [https://vcani.chirmyram.com/](https://vcani.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Ani-orange?&style=flat)](https://vcani.chirmyram.com/)

### 4. 电影盘

- ▶ 4.1 [https://cfdmov.chirmyram.com/](https://cfdmov.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Mov-orange?&style=flat)](https://cfdmov.chirmyram.com/)

- ▶ 4.2 [https://vcmov.chirmyram.com/](https://vcmov.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Mov-orange?&style=flat)](https://vcmov.chirmyram.com/)

### 5. 图书盘

- ▶ 5.1 [https://cfddoc.chirmyram.com/](https://cfddoc.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Doc-orange?&style=flat)](https://cfddoc.chirmyram.com/)

- ▶ 5.2 [https://vcdoc.chirmyram.com/](https://vcdoc.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Doc-orange?&style=flat)](https://vcdoc.chirmyram.com/)

### 6. 剧集一盘

- ▶ 6.1 [https://cfdtlv.chirmyram.com/](https://cfdtlv.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Tlv-orange?&style=flat)](https://cfdtlv.chirmyram.com/)

- ▶ 6.2 [https://vctlv.chirmyram.com/](https://vctlv.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Tlv-orange?&style=flat)](https://vctlv.chirmyram.com/)

### 7. 剧集二盘

- ▶ 7.1 [https://cfdtlv2.chirmyram.com/](https://cfdtlv2.chirmyram.com/) [![](https://img.shields.io/badge/CFW_CFP-brightgreen?&style=flat)](https://www.cloudflare.com/zh-cn/) [![](https://img.shields.io/github/stars/vcheckzen/FODI?style=flat&label=star)](https://logi.im/back-end/fodi-on-cloudflare.html) [![](https://img.shields.io/badge/Tlv2-orange?&style=flat)](https://cfdtlv2.chirmyram.com/)

- ▶ 7.2 [https://vctlv2.chirmyram.com/](https://vctlv2.chirmyram.com/) [![](https://img.shields.io/badge/Vercel-brightgreen?&style=flat)](https://vercel.com/) [![](https://img.shields.io/github/stars/spencerwooo/onedrive-vercel-index?style=flat&label=star)](https://github.com/spencerwooo/onedrive-vercel-index) [![](https://img.shields.io/badge/Tlv2-orange?&style=flat)](https://vctlv2.chirmyram.com/)
