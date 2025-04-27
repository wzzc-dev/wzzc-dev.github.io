---
title: Logseq 博客发布方案
date: '2025-03-25 14:21:50'
updated: '2025-04-27 14:04:28'
permalink: /post/logseq-blog-publishing-solution-ujo8n.html
comments: true
toc: true
---





public:: true
type:: 笔记
item-type:: 软件分享
plane:: done

- # Logseq 博客发布方案
- Logseq 一个双链笔记
- 两种转换成静态页面的方案：
  - 1、通过 Logseq 的导出图谱功能导出静态文件到一个文件夹，github/gitee page 直接部署这个文件夹
  - 2、通过 Logseq Publish Action ，这个时候是推送整个 Logseq 所有文件到 github，然后添加 Logseq Publish Action， github 会自动发布静态页面到另一个分支
    - logseq/publish-spa@v0.3.0
- ~~同时发布到 gitee 和 github~~ gitee已下线page服务
  - 另外可以使用 [git-mirror-action](https://github.com/wearerequired/git-mirror-action) 不同仓库之间同步 ： 首先推送 Logseq 全部文件到 GitHub 一个公开或者私有的库，然后 Logseq Publish Action 来生成静态文件并推送到另一个公开的分支或者库，git-mirror-action 可以同步不同的 git 库，利用 git-mirror-action 将 GitHub 上的库同步到 Gitee，但是 Gitee Page 并不会自动部署，所以要使用 [gitee-pages-action](https://gitee.com/Mikeywk/gitee-pages-action) 自动部署 Gitee Pages
- 评论系统
  - [Logseq 接入评论系统 (abosen.top)](https://logseq.abosen.top/#/page/logseq%20接入评论系统)
- #部署方案#
  - Cloudflare Pages
    - [(wzzc.pages.dev)](https://wzzc.pages.dev/)
  - GitHub Pages
    - [wzzc-dev.github.io](https://wzzc-dev.github.io/)
  - [Vercel](https://vercel.com/)
    - [wzzc.vercel.app/#/page/overview](https://wzzc.vercel.app/#/page/overview)
  - [render](https://render.com/about#)
    - [wzzc.onrender.com](https://wzzc.onrender.com/)
  - [netlify](https://www.netlify.com/)
    - [wzzc.netlify.app](https://wzzc.netlify.app/#/page/overview)
- 参考文档
  - [pengx17/logseq-publish: Logseq Publish Action (github.com)](https://github.com/pengx17/logseq-publish)
  - [All journals (tothegarden.vercel.app)](https://tothegarden.vercel.app/all-journals)
  - [通过 GitHub Actions 实现私有仓库的免费 Github Pages 部署 - 掘金 (juejin.cn)](https://juejin.cn/post/7008847699919241229)
  - [如何发布logseq成为博客 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/344165645)
  - [利用GitHub-Actions将Hugo博客自动发布到GitHub和Gitee Pages - 简书 (jianshu.com)](https://www.jianshu.com/p/7c3f31d44b1d)
  - [gitee-pages-action: 🤖 无须人为干预，自动部署 Gitee Pages](https://gitee.com/heartaotime/gitee-pages-action)
