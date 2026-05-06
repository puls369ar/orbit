# Stack

| Problem you must solve   | Goal at this stage     | Technology to use        | Tech stack (exact tools)        | Language & framework / library      |
| ------------------------ | ---------------------- | ------------------------ | ------------------------------- | ----------------------------------- |
| Know how far objects are | Rough depth estimation | Software stereo depth    | Dual cheap USB cameras + OpenCV | Python / C++ — OpenCV               |
| Know object height       | Precise geometry       | True 3D coordinates      | Depth → PointCloud2             | C++ — ROS 2, PCL                    |
| Detect free space        | Safe navigation        | 2.5D ground segmentation | Costmaps                        | C++ — ROS 2 Costmap2D               |
| Stay stable while moving | Robust motion          | Sensor fusion (EKF)      | `robot_localization`            | C++ — ROS 2                         |
| Know robot position      | Long‑term consistency  | RGB‑D SLAM               | RTAB‑Map                        | C++ — RTAB‑Map, ROS 2               |
| Understand objects       | Safety & semantics     | AI object detection      | YOLO                            | PyTorch (train) / TensorRT (deploy) |
| Run on edge hardware     | Real‑time + low power  | Optimized inference      | TensorRT on Jetson              | C++ — TensorRT                      |
| Move robot safely        | Predictable motion     | Navigation & planning    | Nav2                            | C++ — ROS 2 Nav2                    |
>In production cheap USB cameras will be replaced with more reliable camera such as Intel RealSense D435 using C++ SDK
