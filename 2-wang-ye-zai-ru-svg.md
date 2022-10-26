# 網頁載入 SVG

## 方式一：使用 img 標籤

使用 img 標籤載入 SVG 格式的圖檔：

{% code lineNumbers="true" %}
```html
<img src="./my_img.svg">
```
{% endcode %}

例：

{% embed url="https://codepen.io/carlos411/pen/qBKBzEX" %}



## 方式二：使用 CSS

使用 CSS 載入 SVG 格式的圖檔：

{% code lineNumbers="true" %}
```css
.container1 {
  background-image: url("https://alldata.sgp1.digitaloceanspaces.com/images/head_icon.svg");
  background-size: 150px;
  border: 1px solid grey;
  width: 500px;
  height: 500px;
}
```
{% endcode %}

例：

{% embed url="https://codepen.io/carlos411/pen/xxzxowd" %}



## 方式三：將 SVG 直接寫在 HTML 檔

將 SVG 直接寫在 HTML 檔，且加上動態效果，滑鼠移過時，換顏色。



例：

{% embed url="https://codepen.io/carlos411/pen/ZEREdQW" %}

