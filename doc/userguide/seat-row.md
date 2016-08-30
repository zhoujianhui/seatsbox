
# 多行座位
Seatsbox支持绘制多行多列的圆形和方形座位，也可绘制默认行列数的座位。

## 多行圆形座位
进入多行圆形座位绘制状态
```javascript
designer.toRowOfRoundChairDrawingState();
```
此时鼠标会变为圆形座位形状

![CircleSeatCursor](http://zhoujianhui.bitbucket.org/seatsbox/circleseatcursor.png)

单击并拖拽鼠标即可画出多行多列的圆形座位，如：

![RowOfRoundChair](http://zhoujianhui.bitbucket.org/seatsbox/rowofroundchair.png)

### 配置多行圆形座位绘制器 
在进入绘制状态前**全局设置**：
```javascript
seatsbox.seat.Row.seatWidth = seatsbox.seat.Row.seatHeight = 60;
seatsbox.seat.Row.seatSpace = 20;
```

进入绘制状态后，设置当前绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    seatWidth: 60,
    seatHeight: 60,
    seatSpace: 20
});
```
此时绘制出来的多行圆形座位变为自定义的大小和间隔

![RowOfRoundChairCustom](http://zhoujianhui.bitbucket.org/seatsbox/rowofroundchair-custom.png)


## 多行方形座位
进入多行方形座位绘制状态
```javascript
designer.toRowOfRectChairDrawingState();
```
此时鼠标会变为方形座位形状

![RectSeatCursor](http://zhoujianhui.bitbucket.org/seatsbox/rectseatcursor.png)

单击并拖拽鼠标即可画出多行多列的方形座位，如：

![RowOfRectChair](http://zhoujianhui.bitbucket.org/seatsbox/rowofrectchair.png)

### 配置多行方形座位绘制器 
在进入绘制状态前**全局设置**：
```javascript
seatsbox.seat.Row.seatWidth = 60;
seatsbox.seat.Row.seatHeight = 60;
seatsbox.seat.Row.seatSpace = 20;
```

进入绘制状态后，设置当前绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    seatWidth:60,
    seatHeight:60,
    seatSpace:20
});
```
此时绘制出来的多行方形座位变为自定义的大小和间隔

![RowOfRectChairCustom](http://zhoujianhui.bitbucket.org/seatsbox/rowofrectchair-custom.png)


## 固定行圆形座位
进入固定行圆形座位绘制状态
```javascript
designer.toFixedRowOfRoundChairDrawingState();
```
此时鼠标会变为圆形座位形状

![CircleSeatCursor](http://zhoujianhui.bitbucket.org/seatsbox/circleseatcursor.png)

单击鼠标即可画出固定行列的圆形座位，如：

![FixedRowOfRoundChair](http://zhoujianhui.bitbucket.org/seatsbox/fixedrowofroundchair.png)

### 配置固定行圆形座位绘制器
在进入绘制状态前**全局设置**：
```javascript
seatsbox.drawer.FixedRowDrawer.rowNums=4;
seatsbox.drawer.FixedRowDrawer.colNums=4;
```

进入绘制状态后，设置当前绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
     rowNums:4,
     colNums:4,
     seatWidth:40,
     seatHeight:40,
     seatSpace:20
});
```
此时绘制出来的多行圆形形座位变为自定义的行列数、大小和间隔

![FixedRowOfRectChairCustom](http://zhoujianhui.bitbucket.org/seatsbox/fixedrowofroundchair-custom.png)


## 固定行方形座位
进入固定行方形形座位绘制状态
```javascript
designer.toFixedRowOfRectChairDrawingState();
```

### 配置固定行方形形座位绘制器
参见上文