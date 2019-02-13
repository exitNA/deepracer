## roslaunch deepracer_simulation racecar.launch

* GazeboRosControlPlugin missing `<legacyModeNS>` while using DefaultRobotHWSim, defaults to true.
  * 修改`urdf/racecar.gazebo`文件，在`<plugin name="gazebo_ros_control" filename="libgazebo_ros_control.so">`里插入`<legacyModeNS>true</legacyModeNS>`

* futures requires Python '>=2.6, <3' but the running Python is 3.5.2

  * ```bash
    # 切换到python3
    pip install futures==3.1.1
    ```

* **Deprecated syntax, please prepend 'hardware_interface/'**

  * 在.xacro里的 `<hardwareInterface>`添加hardware_interface/

    例如：

    ```xml
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
    ```

    

