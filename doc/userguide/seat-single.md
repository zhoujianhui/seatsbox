# 单个座位
## 圆形座位
进入单个圆形座位绘制状态
```javascript
designer.toRoundChairDrawingState();
```
此时鼠标会变为圆形座位形状

![CircleSeatCursor](http://zhoujianhui.bitbucket.org/seatsbox/circleseatcursor.png)

单击画布即可画出单个的圆形座位，如：

![CircleSeat](http://zhoujianhui.bitbucket.org/seatsbox/circleseat.png)

### 配置单个圆形座位绘制器
在进入绘制状态前**全局设置**：
```javascript
seatsbox.seat.RoundChair.width = 20;
```

进入绘制状态后，设置当前绘制器的座位大小：
```javascript
designer.drawer.setDrawConfig({
     width:20
});
```
此时鼠标样式会变为自定义的大小

![CircleSeatCursorBig](http://zhoujianhui.bitbucket.org/seatsbox/circleseatcursor-big.png)

绘制出来的圆形座位也相应变为自定义的大小

![CircleSeatBig](http://zhoujianhui.bitbucket.org/seatsbox/circleseat-big.png)


## 方形座位
```javascript
designer.toRectChairDrawingState();
```
此时鼠标会变为方形座位形状

![RectSeatCursor](http://zhoujianhui.bitbucket.org/seatsbox/rectseatcursor.png)

单击画布即可画出单个的方形座位，如：

![RectSeat](http://zhoujianhui.bitbucket.org/seatsbox/rectseat.png)

### 配置单个方形座位绘制器
在进入绘制状态前**全局设置**：
```javascript
seatsbox.seat.RectChair.width = 20;
seatsbox.seat.RectChair.height = 20;
```

进入绘制状态后，设置当前绘制器的座位大小：
```javascript
designer.drawer.setDrawConfig({
     width:20,
     height:20
});
```
此时鼠标样式会变为自定义的大小

![RectSeatCursorBig](http://zhoujianhui.bitbucket.org/seatsbox/rectseatcursor-big.png)

绘制出来的圆形座位也相应变为自定义的大小

![RectSeatBig](http://zhoujianhui.bitbucket.org/seatsbox/rectseat-big.png)