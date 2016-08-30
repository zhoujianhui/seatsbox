# 建筑物（Building）
建筑物是场地中不能用于人员安排的设施，目前含有：

 - 过道
 - 电梯
 - 安全出口


## 过道（Aisle）
进入过道绘制状态
```javascript
designer.toAisleDrawingState();
```

此时鼠标会变为过道形状

![AisleCursor](http://zhoujianhui.bitbucket.org/seatsbox/aislecursor.png)

拖拽即可绘制任意大小的过道，如：

![Aisle](http://zhoujianhui.bitbucket.org/seatsbox/aisle.png)


## 电梯（Elevator）
进入电梯绘制状态
```javascript
designer.toElevatorDrawingState();
```

此时鼠标会变为电梯形状

![ElevatorCursor](http://zhoujianhui.bitbucket.org/seatsbox/elevatorcursor.png)

单击即可绘制固定大小的电梯，如：

![Elevator](http://zhoujianhui.bitbucket.org/seatsbox/elevator.png)

### 设置电梯的绘制大小
SeatsBox对所有的绘制器提供两种配置方式：全局配置和单次绘制配置。

在进入绘制状态前**全局设置**：
```javascript
seatsbox.building.Elevator.width = 49;
seatsbox.building.Elevator.height = 42;
```

进入绘制状态后，设置**当前**绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    width: 49,
    height: 42
});
```
此时鼠标样式会变为自定义的大小

![ElevatorCursorBig](http://zhoujianhui.bitbucket.org/seatsbox/elevatorcursor-big.png)

绘制出来的电梯也相应变为自定义的大小

![ElevatorBig](http://zhoujianhui.bitbucket.org/seatsbox/elevator-big.png)


## 安全出口（EmergencyExit）
进入安全出口绘制状态
```javascript
designer.toEmergencyExitDrawingState();
```

此时鼠标会变为安全出口形状

![EmergencyExitCursor](http://zhoujianhui.bitbucket.org/seatsbox/emergencyexitcursor.png)

单击即可绘制固定大小的安全出口，如：

![EmergencyExit](http://zhoujianhui.bitbucket.org/seatsbox/emergencyexit.png)

### 设置安全出口的绘制大小
在进入绘制状态前**全局设置**：
```javascript
seatsbox.building.EmergencyExit.width = 40;
seatsbox.building.EmergencyExit.height = 40;
```

进入绘制状态后，设置**当前**绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    width: 40,
    height: 40
});
```
此时鼠标样式会变为自定义的大小

![EmergencyExitCursorBig](http://zhoujianhui.bitbucket.org/seatsbox/emergencyexitcursor-big.png)

绘制出来的安全出口也相应变为自定义的大小

![EmergencyExitBig](http://zhoujianhui.bitbucket.org/seatsbox/emergencyexit-big.png)