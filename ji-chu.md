# 座標系統

## 預設的座標系統

{% embed url="https://codepen.io/carlos411/pen/VwKKzEX" %}



## 座標系統：使用 viewBox

width 與 height 的比例，等同於 viewBox。( `400:500 = 64:80` )

可以將 viewBox 想成解析度去調整看看。

`viewBox="0 0 64 80"` 的意思是 0 0 分別是 x 和 y 的座標，64 80 指的是水平方向有 64 個點和垂直方向有 80 個點。

{% embed url="https://codepen.io/carlos411/pen/poexjWo" %}



## preserveAspectRatio

當 width 與 height 的比例不等於 viewBox 時，才會有效。

預設值是 **`xMidYMid meet`**。分別是以下三個：

* 有 xMin、xMid、xMax。
* 有 YMin、YMid、YMax。
* 有 meet、slice、none。(如果是設定 none 的話，那就 `preserveAspectRatio="none"` 這樣寫即可，表示會變形，會強制壓縮在 viewport 範圍內)。



下例，可以試著將 height 改成 400px，然後改 `preserveAspectRatio` 屬性試試。

{% embed url="https://codepen.io/carlos411/pen/abJRqBx" %}



## 巢狀式的 SVG 及座標系統

{% embed url="https://codepen.io/carlos411/pen/PopyQvE" %}



