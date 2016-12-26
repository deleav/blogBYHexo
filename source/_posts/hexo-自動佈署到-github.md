title: hexo 佈署到 github
date: 2016-03-04 06:04:19
categories: 開發環境
tags: hexo
---

![燈塔](/imgs/img2.jpg)

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
  * 以下兩個都是先產生檔案再部署的意思
    ```bash
    // 以下二選一
    hexo g -d
    hexo d -g
    // d(deploy), g(generate) --> 簡寫(原始指令)
    ```

# ref.
  * [Hexo Deployment](https://hexo.io/docs/deployment.html)
  * [Hexo Generating](https://hexo.io/docs/generating.html)
