title: atom package backup
date: 2016-03-04 04:54:33
categories:
  - 開發環境
tags:
  - atom
  - coding
---

![早晨](/imgs/atom-package-backup.jpg)

<!-- more -->

# 如何備份 atom package lists
  * backup
    ```bash
    apm list --installed --bare > packages.list
    ```
    會在當前目錄下產生 packages.list

  * install all
    ```bash
    apm install `cat packages.list`
    ```

# My atom package list

* [package.list](https://github.com/deleav/atom-setting-backup/blob/master/packages.list)

```json
atom-beautify@0.29.6
atom-jade@0.3.0
autocomplete-modules@1.4.1
autocomplete-paths@1.0.2
emmet@2.4.3
file-icons@1.7.5
highlight-selected@0.11.2
language-babel@2.17.3
language-ejs@0.2.0
markdown-preview-plus@2.4.0
merge-conflicts@1.4.1
pigments@0.26.0
project-manager@2.9.7
react@0.15.0
```

# ref.
  * [How to backup all your atom setting](https://discuss.atom.io/t/how-to-backup-all-your-settings/15674)
