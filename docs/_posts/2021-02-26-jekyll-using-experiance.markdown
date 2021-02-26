---
layout: post
title:  "Jekyll 初步使用心得"
date:   2021-02-26 12:55:00 +0800
categories: web framework note
---

Jekyll 用了大概兩天，基本概念大概抓到了。

簡單的說 Jekyll 是一個幫忙生成靜態網頁的 Framework。

在網頁的資料夾內，放入所有想要的資料與設定，之後會在 _site 中產生最後成果。

所有的 Blog 資料可以放到 _post 的資料夾中，如果網頁想要修改，不想與其他人一樣，可以在 _layouts 中修改。

_config.yml 中放了所有網頁的 header 與 footer 的基本資料。

算是架設網頁很方便的小工具，再加上 Github Page 有支援，讓想架設 Blog 的普通人省了很多心力。

以下是 Jekyll 產生出的檔案架構

```bash
docs
   ├───_layouts
   ├───_posts
   ├───_site
   ├───Gemfile
   └───_config.yml
```