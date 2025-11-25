 
# ROS2 Delivery Bypass Script

[+] This script fixes the **bottle pickup failure bug** in ROS2 delivery.

For detailed technical analysis, please refer to the PDF:
[+] Official program defect analysis
[+] Subscription node bypass

---

# Build & Run

```bash
$ cd ~/ros2_ws
```

```bash
$ colcon build
```

---

![alt text](./pic/image.png)

Load the map:

```bash
$ cp ./waypoints.yaml ~;cp -r ./maps /home/two/ros2_ws/src/wpr_simulation2/maps
```

Load the environment:

```bash
$ source install/setup.bash
```

Launch the simulation:

```bash
$ ros2 launch home_pkg home.launch.py
```

---

Add robot orientation:

![alt text](./pic/image-1.png)

Start the exploit tool:

```bash
$ python3 bypass.py
```

---

![alt text](./pic/image-2.png)

![alt text](./pic/image-3.png)

![alt text](./pic/image-4.png)

![alt text](./pic/image-5.png)

---
 
