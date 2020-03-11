---
layout: post
title: Maverick搭建过程
slug: 博客搭建
date: 2020-03-11 09:34
status: publish
author: <Reedmark>
categories: 
  - 默认分类
tags: 
  - 博客
  - GitHub
excerpt: 
---

#### 1.fork https://github.com/AlanDecode/Blog-With-GitHub-Boilerplate这个仓库

#### 2. 下载gh-pages分支的所有内容，并重新上传到新分支master上

#### 3. 为仓库添加一个 token并加入 Setting中的 Secrets 上

#### 4. 修改仓库名为 `<用户名.github.io>` 的形式

#### 5.在 conf.py 中将 `site_prefix` 修改为 `"/"`

#### 6.修改 .github/workflows/ci.yml 第 55 行为 `PUBLISH_BRANCH: master`

#### 7. 开启Actions

#### 8.点击 conf.py 文件，然后点击编辑按钮。修改 `enable_jsdelivr` 如下：

```
enable_jsdelivr = {
    "enabled": True,
    "repo": "RuomingBai/RuomingBai.github.io@master"
}
```

