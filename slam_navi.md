启动世界地图

```shell
roslaunch turtlebot3_gazebo turtlebot3_world.launch
```

开始扫描建图

```shell
roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
```

键盘控制机器人

```shell
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
```

存储扫描的地图

```shell
rosrun map_server map_saver -f ~/map
```

导入扫描的地图

```shell
roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
```



