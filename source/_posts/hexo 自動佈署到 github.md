title: hexo 佈署到 github
date: 2016-03-04 06:04:19
categories: 開發環境
tags: hexo
---

![Brick wall](https://pixabay.com/static/uploads/photo/2016/03/16/11/16/background-1260304_960_720.jpg)

<!-- more -->

# 如果你已經架設好 hexo 了
  * install `hexo-deployer-git`
  * 設定 `_config.yml`
    ```yml
    deploy:
      type: git
      repo: https://github.com/username/repo
      branch: branch // master or gh-pages
      message: message // 預設是 Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}
    ```
  * 以下兩個都是 Deploy After Generating 的意思
    ```bash
    // 以下二選一
    hexo g --d
    hexo d --g
    // d(deploy), g(generate) --> 簡寫(原始指令)
    ```
