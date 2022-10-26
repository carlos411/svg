# rect

## 使用 rect 畫矩形

* x、y 指的是座標。
* 畫矩形時，預設上會填滿黑色，也就是 `fill: black;`。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  
  <rect x="10" y="10" width="30" height="50" />

  <rect x="50" y="10" width="20" height="40" style="fill: none; stroke: black;" />
  
  <rect x="10" y="70" width="25" height="30" style="fill: #0000ff; stroke: red; stroke-width: 7; stroke-opacity: 0.5;" />
  
  <rect x="50" y="70" width="35" height="20" style="fill: yellow; fill-opacity: 0.5; stroke: green; stroke-width: 2; stroke-dasharray: 5 2;" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/zYZMwZM" %}



## 矩形樣式

* `fill`：填滿顏色，預設是 `black`，如果不想有顏色，可設定 `none`。
* `fill-opacity`：填滿顏色的不透明度。



## 設定圓角

* 使用 rx 和 ry 來設定圓角。
* 如果僅設定 rx 或僅設定 ry 的話，那就代表 rx 和 ry 的數值是相等的。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200">
  <rect x="10" y="10" width="20" height="40" rx="2" ry="2" style="stroke: black; fill: none;" />

  <rect x="40" y="10" width="20" height="40" rx="5" style="stroke: black; fill: none;" />

  <rect x="70" y="10" width="20" height="40" ry="10" style="stroke: black; fill: none;" />

  <rect x="10" y="60" width="20" height="40" rx="10" ry="5" style="stroke: black; fill: none;" />

  <rect x="40" y="60" width="20" height="40" rx="5" ry="10" style="stroke: black; fill: none;" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/qBrQmxe" %}

示意圖：

![](../.gitbook/assets/rounded\_rectangles.png)



