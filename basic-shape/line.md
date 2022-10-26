# line

## 使用 line 畫直線

* x1、y1 是直線的起點座標。
* x2、y2 是直線的終點座標。
* 畫線時，線的位置會是在格線系統當中格線的中間。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <line x1="40" y1="20" x2="80" y2="20" style="stroke-width: 10px; stroke: black; stroke-opacity: .5;" />
  <line x1="30" y1="30" x2="85" y2="85" style="stroke: black; stroke-dasharray: 9, 3, 5;" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/gOmQwoN" %}



## 直線樣式

* `stroke`：線的顏色。
* `stroke-width`：線的粗細。
* `stroke-opacity`：線的不透明度。
* `stroke-dasharray`：虛線。(可設定 `9, 5` 以及 `9, 3, 5` 觀察看看，以 9, 3, 5 來說，就是 9px 的線、3px 的間隔、5px 的線、9px 的間隔、3px 的線、5px 的間隔，這樣交錯)

