# defs 元素

## 使用 defs 標籤

上述的 `<use>` 有以下幾個問題：

* 是從原來的位置去做位移，很麻煩。
* 無法建立不同顏色的房止，因為使用 `<use>` 的話，無法覆蓋原來的 CSS。
* 一定要畫一次 house、man、woman。

使用 `<defs>` 可以解決上述問題。`<defs>` 是用來定義一組圖案，然後並不會顯示在畫面上，若要顯示，可搭配使用 `<use>` 標籤。

例：

{% embed url="https://codepen.io/carlos411/pen/jOBRZwO" %}

