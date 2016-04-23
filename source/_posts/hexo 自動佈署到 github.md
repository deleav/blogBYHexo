title: hexo 自動佈署到 github
date: 2016-03-04 06:04:19
categories: 開發環境
tags: hexo
---

![Brick wall](https://pixabay.com/static/uploads/photo/2016/03/16/11/16/background-1260304_960_720.jpg)

<!-- more -->

# 如果你已經架設好 hexo 了
  * install `hexo-deployer-git`
  * 設定 `_config.yml`
    * ssh
      ```yml
      deploy:
        type: git
        repo: git@github.com:username/repo
        branch: branch // master or gh-pages
        message: message // 預設是 Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}
      ```
      <!-- * 請注意須要先有在 github 新增 ssh key (若無請參考 [如何在 github 上新增 ssh key](https://help.github.com/articles/generating-an-ssh-key/)) -->

    <!-- * https
      ```yml
      deploy:
        type: git
        repo: https://github.com/username/repo
        branch: gh-pages // 或 repo name 是 username.github.io 就用 master
        message: message // 預設是 Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}
      ``` -->
