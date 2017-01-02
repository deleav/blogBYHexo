title: 子元素如何不繼承 CSS 的 opacity 屬性
date: 2017-01-01 22:35:08
tags: CSS
---

![樹](/imgs/do-not-inherit-opacity/tree.jpg)

<!-- more -->

# 事情是這樣的
我想為我的小專案製作一個 Menu 選單，為了讓選單滑出來的時候其他部分是黑色半透明的，我打算放一個全畫面的 `div` 上去，然後上面再放上我的 Menu，所以我這麼做。
```CSS
// menu page css
background-color: black;
opacity: 0.5;
```
結果連 Menu page 上面的子元素全都繼承了 `opacity: 0.5;`，而且在子元素加上 `opacity: 1;` 也完全沒有用，只能在父元素的透明度基礎上更淡。
  * #### 理想
  ![理想](/imgs/do-not-inherit-opacity/img1.jpg)
  * #### 實際
  左邊的 `item1` 跟底色都變淡了，連陰影效果都跟著掛了。
  ![實際](/imgs/do-not-inherit-opacity/img2.jpg)

# 解決方法
其實很簡單，只要改用這種方式來避免更改到 `opacity` 屬性，就不會有改不掉的問題。

```CSS
background-color: rgba(0, 0, 0, 0.5);
// rgba() 前三個值為 R G B，第四個為透明度
```

同理，文字顏色一樣可以這麼做，可惜我還是沒找到能夠複寫父元素的 `opacity` 的方法，等找到了再來更新。
