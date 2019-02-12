## 创建ROS workspace

```bash
# 创建工作目录catkin_ws
mkdir -p catkin_ws/src
cd catkin_ws
catkin_make # 在src目录下创建一个CMakeLists.txt软链接，同时创建build，devel目录

source devel/setup.sh # 引用当前工作目录到环境变量中
```

## ROS 组件

* Node
  * ROS执行节点

* roscore
  * 包含Master，rosout，参数服务器

