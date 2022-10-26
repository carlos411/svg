# use 元素

## 使用 use 標籤來重覆使用

* 透過 `xlink:href` 指定要重覆使用哪個元素。
* 然後透過 x、y 來移動到哪個位置(是相對於原來的元素的位置)。

```markup
<svg width="240px" height="240px" viewBox="0 0 240 240" xmlns="http://www.w3.org/2000/svg">
  <g id="house">
    <!-- other element -->
  </g>
  <g id="man">
    <!-- other element -->
  </g>
  <g id="woman">
    <!-- other element -->
  </g>
  
  <!-- 重覆使用以上圖形，並移動位置 -->
  <use xlink:href="#house" x="70" y="100" />
  <use xlink:href="#woman" x="-80" y="100" />
  <use xlink:href="#man" x="-30" y="100" />
</svg>
```

例：

{% embed url="https://codepen.io/carlos411/pen/VwpRNxW" %}

