# Paths

d 屬性代表是 data 的意思。

M：代表 `moveto`。後面緊接著是座標，可以是空格或逗號做區隔。大寫代表**絕對座標**。

L：代表 `lineto`。後面緊接著是座標，可以是空格或逗號做區隔。大寫代表**絕對座標**。

Z：代表畫回原點。形成一個封閉圖形。

C：curve to。

S：smooth curve to。



## 範例1

{% embed url="https://codepen.io/carlos411/pen/QWgaXLE?editors=1100" %}



## 範例2：封閉圖形

{% embed url="https://codepen.io/carlos411/pen/qBjpzdM" %}



## 範例3：封閉圖形最後使用 Z 和 L 的差別

{% embed url="https://codepen.io/carlos411/pen/wvepLGM" %}



## 範例4：小寫的相對位置

以下兩個 path 畫出來的都是一樣的，大寫是絕對位置，小寫是相對位置：

```markup
<path d="M 10 10 L 20 10 L 20 30  M 40 40 L 55 35" style="stroke: black;" />
<path d="M 10 10 l 10  0 l  0 20  m 20 10 l 15 -5" style="stroke: black;" />
```

例：

{% embed url="https://codepen.io/carlos411/pen/qBjYLbQ" %}

註1：如果最一開始是使用小寫的 m，那會被視為是絕對位置。\
註2：Z(closed path) 的部份，大小寫沒有差別。



## 路徑的簡寫形式



### 範例1：畫水平線、垂直線

* H：代表的是畫水平線，是絕對位置。
* h：代表的是畫水平線，是相對位置。
* V：代表的是畫垂直線，是絕對位置。
* v：代表的是畫垂直線，是相對位置。

例如下例，是畫矩形：

{% embed url="https://codepen.io/carlos411/pen/vYZjvmB" %}

