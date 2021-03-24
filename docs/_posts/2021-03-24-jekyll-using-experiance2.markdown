---
layout: post
title:  "Jekyll 如何控制要展現的Post"
date:   2021-02-26 12:55:00 +0800
categories: web framework note
---

Jekyll 有一個 Singleton 就是 ```site```，呼叫所有的 Post 就是  ```site.posts```

舉個例子，如果想只顯示兩個 Post 可以使用下列方式
```angular2html
{% for post in site.posts limit:2  %}
    //do something
{% endfor %}
```

如果只想顯示特殊類別的 Post，可以利用 ```categories``` 或是 ```tags```

下面是 categories 的範例在自己的 Post 裡面包涵 categories 的資訊
```angular2html
---
layout: post
title: my personal post
categories: Personal
---
```


然後再 HTML 中選擇所有跟```Personal```有關的Post
```angular2html
{% for post in site.categories.Personal %}
<li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
```