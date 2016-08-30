# 宾馆房间
宾馆的绘制会用到上文提到的建筑物绘制，这里只介绍宾馆房间的绘制。

进入宾馆房间绘制状态
```javascript
designer.toHotelRoomDrawingState();
```
此时鼠标会变为

![HotelRoomCursor](http://zhoujianhui.bitbucket.org/seatsbox/hotelroomcursor.png)

单击即可绘制宾馆房间

![HotelRoom](http://zhoujianhui.bitbucket.org/seatsbox/hotelroom.png)

## 宾馆房间配置 
在进入绘制状态前**全局设置**：
```javascript
seatsbox.hotel.HotelRoom.width = 160;
seatsbox.hotel.HotelRoom.height = 80;
seatsbox.hotel.HotelRoom.seatCapacity = 1;
seatsbox.hotel.HotelRoom.roomType = '单人间';
```

进入绘制状态后，设置绘制器的配置：
```javascript
designer.drawer.setDrawConfig({
    width: 160,
    height: 80,
    seatCapacity: 1,
    roomType: '单人间'
});
```
单击即可绘制宾馆房间

![HotelRoomCustom](http://zhoujianhui.bitbucket.org/seatsbox/hotelroom-custom.png)
