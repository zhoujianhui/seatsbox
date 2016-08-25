# 设计器
```javascript
var designer = new seatsbox.Designer();
```
设计器默认全屏并显示在页面的body元素的中。

同时支持设置设计器的大小和所在元素
```html
<body>
<div id='divDesigner'></div>
</body>
```

```javascript
var config= {
    canvasId:'divDesigner',
    width:800,
    height:600
}

var designer = new seatsbox.Designer(config);
```