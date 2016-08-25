# SeatsBox
SeatsBox用于各种场地平面图的绘制和场地的人员安排，适合会场、宾馆、餐厅的绘制及排座，并可将场地导出为模版用于下一次活动的人员安排。


## Business Features

 - 支持会场及餐厅多种座位绘制（圆形、方形座位、圆桌、方桌座位）
 - 支持拖拽绘制多行圆形、方形座位
 - 支持建筑物平面图绘制（过道、电梯、安全出口、指北针）
 - 支持宾馆房间及床位绘制


## Technology Features

 - 采用OOA&D&P, 建立业务领域概念，易于扩展和维护
    - 内置OO实现
    - 内置事件总线
 - 采用多种Agile Practices: TDD,  CI (Jasmine+Karma+Gulp)
 - 采用d3.js作为SVG绘制库，并扩展支持使用SVG图标文件作为自定义绘制类型


## QuickStart
引用seatsbox.js及其依赖的js
```html
<link rel="stylesheet" type="text/css" href="lib/seatsbox.min.css">
<script src="lib/q.min.js"></script>
<script src="lib/lodash.min.js"></script>
<script src="lib/d3.min.js"></script>
<script src="lib/seatsbox.min.js"></script>
```

新建场地设计器
```javascript
var designer = new seatsbox.Designer();
```

进入绘图状态
```javascript
designer.toRoundChairDrawingState();
```

绘制完成，导出场地地图
```javascript
designer.exportSeatsMap();
```
导出的数据为json对象，你可以保存为文件也可保存到数据库

在业务系统中加载场地地图，进行人员安排
```javascript
designer.loadSeatsMap('seatsmap.json')
            .then(function () {
                designer.showSeatContainerNums();
                designer.toSeatArrangingState();
            });
```


## User Guide
参见：《[用户指南](doc/userguide/README.md)》


## Developer Guide
参见：《[开发者指南](doc/developerguide/README.md)》