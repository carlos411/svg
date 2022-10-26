# Transform

主要是在改變座標系統。

## translate

座標系統的移動。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200">
  <g id="square">
    <rect x="0" y="0" width="20" height="20" style="fill: none; stroke:black; stroke-width: 2;" />
  </g>
  <use xlink:href="#square" style="transform: translate(50px, 50px);" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/KKWOrWP" %}

參考：[http://oreillymedia.github.io/svg-essentials-examples/ch06/translate.html](http://oreillymedia.github.io/svg-essentials-examples/ch06/translate.html)

示意圖：

![](.gitbook/assets/transform\_translate.png)

## scale

座標系統的縮放。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200">
  <g id="square">
    <rect x="10" y="10" width="20" height="20" style="fill: none; stroke:black;" />
  </g>
  <use xlink:href="#square" style="transform: scale(2);" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/gOWYOQq" %}

參考：[http://oreillymedia.github.io/svg-essentials-examples/ch06/scale.html](http://oreillymedia.github.io/svg-essentials-examples/ch06/scale.html)

示意圖：(原座標是淺灰色，放大兩倍之後，深黑色是新座標系統。畫的矩形邊框粗細也會跟著放大兩倍)

![](.gitbook/assets/transform\_scale.png)



## 先後順序

先進行 translate，再進行 scale：

{% embed url="https://codepen.io/carlos411/pen/MWmgdrP" %}

示意圖：

![](.gitbook/assets/transform\_translate\_scale.png)

先進行 scale，再進行 translate：

{% embed url="https://codepen.io/carlos411/pen/MWmgdQP" %}

示意圖：

![](.gitbook/assets/transform\_scale\_translate.png)



## 笛卡兒座標系統

{% embed url="https://codepen.io/carlos411/pen/poPoVyj" %}



## rotate

座標系統的旋轉。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200">
  <!-- axes -->
  <polyline points="100 0, 0 0, 0 100" style="stroke: black; fill: none;" />

  <!-- normal and rotated square -->
  <rect x="70" y="30" width="20" height="20" style="fill: gray;" />
  <rect x="70" y="30" width="20" height="20" transform="rotate(45)" style="fill: black;" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/abWbjXB" %}

參考：[http://oreillymedia.github.io/svg-essentials-examples/ch06/rotate.html](http://oreillymedia.github.io/svg-essentials-examples/ch06/rotate.html)

示意圖：

![](.gitbook/assets/svg\_transform\_rotate.png)



基於某個點的旋轉。

```markup
<svg width="200px" height="200px" viewBox="0 0 200 200">
  <!-- center of rotation -->
  <circle cx="50" cy="50" r="3" style="fill: black;" />

  <!-- non-rotated arrow -->
  <g id="arrow" style="stroke: black;">
    <line x1="60" y1="50" x2="90" y2="50" />
    <polygon points="90 50, 85 45, 85 55" />
  </g>

  <!-- rotated around center point -->
  <use xlink:href="#arrow" transform="rotate(60, 50, 50)" />
  
  <use xlink:href="#arrow" transform="rotate(-90, 50, 50)" />
  <use xlink:href="#arrow" transform="rotate(-150, 50 50)" />
</svg>
```

`transform="rotate(60, 50, 50)"` 指的是`旋轉 60 度`，然後是以`座標(50, 50)`為圓心來旋轉。

例

{% embed url="https://codepen.io/carlos411/pen/yLbLqdy" %}



參考：[http://oreillymedia.github.io/svg-essentials-examples/ch06/rotate-center.html](http://oreillymedia.github.io/svg-essentials-examples/ch06/rotate-center.html)



## 基於某個中心點來放大

{% embed url="https://codepen.io/carlos411/pen/LYyYJpO" %}



## skew

skewX 和 skewY：

{% embed url="https://codepen.io/carlos411/pen/NWjrYMG" %}



參考：[http://oreillymedia.github.io/svg-essentials-examples/ch06/skew.html](http://oreillymedia.github.io/svg-essentials-examples/ch06/skew.html)

示意圖：

![](.gitbook/assets/transform\_skewX.png)

