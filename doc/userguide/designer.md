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


## 设置设计器背景
设计器的背景通过样式**.seatsbox-canvas**来设置，默认使用网格图片
```
.seatsbox-canvas {
    background-image: url('grid.png');
}
```
![Designer](http://zhoujianhui.bitbucket.org/seatsbox/designer.png)