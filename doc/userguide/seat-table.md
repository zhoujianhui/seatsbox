# 桌子座位
桌子座位指的是一张桌子搭配四周一圈椅子的座位类型，分为：

 - 圆桌
 - 方桌


## 圆桌座位
进入圆桌座位绘制状态
```javascript
designer.toRoundTableDrawingState();
```
此时鼠标会变为圆桌座位形状

![RoundTableCursor](http://zhoujianhui.bitbucket.org/seatsbox/roundtablecursor.png)

单击鼠标即可画出单个圆桌座位，如：

![RoundTable](http://zhoujianhui.bitbucket.org/seatsbox/roundtable.png)

### 配置圆桌座位
在进入绘制座位状态前**全局设置**：
```javascript
seatsbox.seat.RoundTable.width = 180; // 桌子的大小
seatsbox.seat.RoundTable.seatCapacity = 10; //椅子的个数
seatsbox.seat.RoundTable.seatWidth = seatsbox.seat.RoundTable.seatHeight = 60; //椅子的大小
```

进入绘制座位状态后，设置当前绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    width: 180,
    seatCapacity: 10,
    seatWidth: 60,
    seatHeight: 60
});
```
此时鼠标样式会变为自定义的配置

![RoundTableCursorCustom](http://zhoujianhui.bitbucket.org/seatsbox/roundtablecursor-custom.png)

绘制出来的圆桌座位也相应变为自定义的配置

![RoundTableCustom](http://zhoujianhui.bitbucket.org/seatsbox/roundtable-custom.png)


## 方桌座位
进入方桌座位绘制状态
```javascript
designer.toRectTableDrawingState();
```
此时鼠标会变为方桌座位形状

![RectTableCursor](http://zhoujianhui.bitbucket.org/seatsbox/recttablecursor.png)

单击鼠标即可画出单个方桌座位，如：

![RectTable](http://zhoujianhui.bitbucket.org/seatsbox/recttable.png)

### 配置方桌座位
在进入绘制状态前**全局设置**：
```javascript
seatsbox.seat.RectTable.seatWidth = 60;
seatsbox.seat.RectTable.seatHeight = 60;
seatsbox.seat.RectTable.seatSpace = 30; // 指定首尾座位和方桌边之间的间距

// 分别设置上下左右边的座位个数和间隔
seatsbox.seat.RectTable.topSideSeatCapacity = 6;
seatsbox.seat.RectTable.topSideSeatSpace = 20;

seatsbox.seat.RectTable.downSideSeatCapacity = 4;
seatsbox.seat.RectTable.downSideSeatSpace = 10;

seatsbox.seat.RectTable.leftSideSeatCapacity = 1;
seatsbox.seat.RectTable.leftSideSeatSpace = 10;

seatsbox.seat.RectTable.rightSideSeatCapacity = 2;
seatsbox.seat.RectTable.rightSideSeatSpace = 10;
```

进入绘制座位状态后，设置当前绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    seatWidth: 60,
    seatHeight: 60,
    seatSpace: 30,
    topSideSeatCapacity: 6,
    topSideSeatSpace: 20,
    downSideSeatCapacity: 4,
    downSideSeatSpace: 10,
    leftSideSeatCapacity: 1,
    leftSideSeatSpace: 10,
    rightSideSeatCapacity: 2,
    rightSideSeatSpace: 10
});
```
此时鼠标样式会变为自定义的配置

![RectTableCursorCustom](http://zhoujianhui.bitbucket.org/seatsbox/recttablecursor-custom.png)

绘制出来的方桌座位也相应变为自定义的配置

![RectTableCustom](http://zhoujianhui.bitbucket.org/seatsbox/recttable-custom.png)