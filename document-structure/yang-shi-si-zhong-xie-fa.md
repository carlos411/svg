# 樣式四種寫法

## Inline Styles

直接寫在 style 屬性上。例：

```markup
<circle cx="20" cy="20" r="10" style="stroke: black; stroke-width: 1.5; fill: blue; fill-opacity: 0.6" />
```



## Internal Stylesheets

以下 CodePen 展示了 Internal Stylesheets 的寫法：

{% embed url="https://codepen.io/carlos411/pen/NWpJaqQ" %}



## External Stylesheets

以下 CodePen 展示了 External Stylesheets 的寫法：

{% embed url="https://codepen.io/carlos411/pen/JjWzrRO" %}



## Presentation Attributes

此例：

```markup
<circle cx="10" cy="10" r="5" style="fill: red; stroke:black; stroke-width: 2;" />
```

可以改寫成(這就是 Presentation Attributes)的寫法(不建議使用)：

```markup
<circle cx="10" cy="10" r="5" fill="red" stroke="black" stroke-width="2" />
```

