---
layout: post
title:  "Jekyll setup for Mac M1"
date:   2021-03-09 16:26:00 +0800
categories: jekyll update
---

終於把 Jekyll 成功地安裝到 Mac 上面了，我原本的計畫就是這台電腦是準備拿來寫自己的東西。

所以如果有工具無法在Mac上使用會讓我很困擾。不過嚐鮮的代價便是有很多程式目前不支援ARM架構，或是可以支援但是很難找到討論。

我所遇到的問題就是正常的Homebrew沒辦法正常安裝ruby在Mac上，安裝3.0的ruby最後還是看到ruby 2.6。

解決方式正常安裝Homebrew，但是ruby必須是2.7，而且在前面要加 ```arch -arm64``` 之後在 ```~/.zshrc```中加上```export PATH="/opt/homebrew/opt/ruby@2.7/bin:$PATH"```
``` 
arch -arm64 brew reinstall ruby@2.7
```

之後就正常安裝 Jekyll 就可以了