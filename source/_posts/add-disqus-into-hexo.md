title: 在 Hexo 使用 Disqus 評論功能
date: 2017-01-02 19:30:36
tags:
  - hexo
  - disqus
---

![廚房](/imgs/add-disqus-into-hexo/kitchen.jpg)

<!-- more -->

# 申請帳號
首先，你需要先到 [Disqus](https://disqus.com/) 申請一個帳號。

# 新增 Site
登入後在首頁右上角點 Admin，然後在左上角選擇 Your Site 點 New

![](/imgs/add-disqus-into-hexo/img1.jpg)
然後在這邊打上你想要的 shortname，然後選個 Category

![](/imgs/add-disqus-into-hexo/img2.jpg)
接下來的都不管他，一直下一步到結束，然後選上面的 setting

![](/imgs/add-disqus-into-hexo/img3.jpg)
可以看到這裡有寫
> Your website shortname is testeeee-1

把他加在你 hexo 的 `_config.yml`

```yml
# Disqus
disqus_shortname: testeeee-1
```
就能開始使用 disqus 提供的評論功能了，這邊是因為有跟別人重複到 shortname，所以他強制加了 `-1`，如果沒有重複到的話就會是你原本設定的那個 shortname 了。
