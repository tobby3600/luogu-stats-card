> 注意：为了不滥用洛谷服务器流量，本项目利用 vercel 的边缘缓存功能缓存了 12 小时数据，即同一个用户卡片 **24 小时内最多只会向洛谷服务器请求 2 次数据**，并且只有在用户访问卡片时才会请求数据。

# 注意：

这个项目不是我的，我只是为了方便用才部署的，原链接：https://github.com/wao3/luogu-stats-card

## 简介

![stars](https://badgen.net/github/stars/wao3/luogu-stats-card?cache=600)
![forks](https://badgen.net/github/forks/wao3/luogu-stats-card?cache=600)
![visitor](https://visitor-badge.laobi.icu/badge?page_id=luogu-stats-card)
![last commit](https://badgen.net/github/last-commit/wao3/luogu-stats-card?cache=600)
![top language](https://img.shields.io/github/languages/top/wao3/luogu-stats-card)

`luogu-stats-card`是一个动态生成洛谷用户练习数据卡片的工具，可以展示自己的做题情况。可以用于个人主页、博客、github等可以插入图片的地方。

## 效果预览

[![Tobby3600的练习情况](https://luogu-userinfo-find-tobby.vercel.app/api?id=426462&dark_mode=true&card_width=750)](https://www.luogu.com.cn/user/426462)
[![Tobby3600的咕值情况](https://luogu-userinfo-find-tobby.vercel.app/guzhi?id=426462&dark_mode=true&card_width=750&scores=100,10,0,0,0)]

## 如何使用

### 练习情况

练习情况可以自动获取用户的数据，但是前提是没有开启“完全隐私保护”，具体使用方法如下：

1. 仅使用图片：直接复制以下内容到任意 markdown 编辑器中，并将`?id=`后面的数字更改为自己的 id 即可（id是洛谷个人主页地址的一串数字）。

   ```markdown
   ![tobby3600的练习情况](https://luogu.vercel.app/practice?id=426462)
   ```

2. 使用图片链接：复制以下内容，第二个小括号内的地址是点击该图片跳转的地址，建议设置为洛谷个人主页。

   ```markdown
   [![tobby3600的练习情况](https://luogu.vercel.app/practice?id=426462)](https://github.com/wao3/luogu-stats-card)
   ```

### 咕值信息

咕值信息无法自动获取数据，如果需要必须要提供 cookie ，但是 这种方法十分不安全，并且不方便，所以获取咕值卡片需要手动输入咕值信息，具体使用方法如下。

复制以下内容到任意 markdown 编辑器中，并将 `?id=`后面的数字更改为自己的 id，将`scores=`后面更换为自己的咕值信息，一共 5 个数字，用逗号分隔。

1. 仅使用图片：复制以下内容到任意 markdown 编辑器中，并将 `?id=`后面的数字更改为自己的 id，将`scores=`后面更换为自己的咕值信息，一共 5 个数字，用逗号分隔。

   ```markdown
   ![tobby3600的咕值信息](https://luogu-userinfo-find-tobby.vercel.app/guzhi?id=426462&scores=100,65,45,15,0)
   ```

2. 使用图片链接：复制以下内容，第二个小括号内的地址是点击该图片跳转的地址，建议设置为洛谷个人主页。

   ```markdown
   [![tobby3600的咕值信息](https://luogu-userinfo-find-tobby.vercel.app/guzhi?id=426462&scores=100,65,45,15,0)](https://github.com/wao3/luogu-stats-card)
   ```


### 自定义选项

使用卡片时，支持设定自定义效果选项，可以组合使用。

1. **隐藏标题**，只需在链接最后带上`&hide_title=true`即可，例如：

   ```markdown
   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&hide_title=true)
   ```

   效果：

   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&hide_title=1)

2. **黑暗模式**，只需在链接最后带上`&dark_mode=true`即可，例如：

   ```markdown
   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&dark_mode=true)
   ```

   效果：

   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&dark_mode=1)

3. **自定义宽度**，默认500，限制宽度在500到1920之间，只需在链接最后带上`&card_width=需要的宽度`即可，例如：

   ```markdown
   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&card_width=750)
   ```

   效果：

   ![tobby3600的练习情况](https://luogu.vercel.app/api?id=426462&card_width=750)

## 自行部署



我就是这么部署的...

部署到自己的 vercel 服务器，登录 [vercel](https://vercel.com/) 后，点击下方按钮即可部署。

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/wao3/luogu-stats-card)

## LICENSE

[![MIT License](https://badgen.net/github/license/wao3/luogu-stats-card)](https://github.com/wao3/luogu-stats-card/blob/master/LICENSE)
