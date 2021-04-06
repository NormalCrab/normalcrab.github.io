---
layout: post
title:  "Jekyll 利用 categories 控制 想要展現的 Post"
date:   2021-04-06 12:55:00 +0800
categories: web framework note
---

在每個Post 開頭都會放一些設定`categories` 可以 filter 一些自己不想顯示的 Post
```angular2html
---
layout: post
title:  "Jekyll 利用 categories 控制 想要展現的 Post"
date:   2021-04-06 12:55:00 +0800
categories: web framework note
---

```

如果我只想顯示`categories`中 `web` 的分類，我可以用底下的範例
```angular2html
 {% assign posts = site.categories.web %}
```