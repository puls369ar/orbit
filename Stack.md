

|Problem you must solve|Why it exists in the real world|Technology to use|Tech stack (exact tools)|Language & framework / library|
|---|---|---|---|---|
|Know how far objects are|Images don’t contain distance|Stereo depth|Intel RealSense D435 + RealSense SDK|C++ / Python — RealSense SDK|
|Know object height|2D can’t separate floor vs obstacle|3D coordinates (XYZ)|Depth → PointCloud2 (ROS 2)|C++ — ROS 2, PCL|
|Detect free space|Robot must know drivable area|Ground segmentation (2.5D)|Depth projection → costmap|C++ — ROS 2 Costmap2D|
|Stay stable while moving|Depth is noisy frame‑to‑frame|Sensor fusion|`robot_localization` (EKF)|C++ — ROS 2|
|Know robot position over time|Motion causes drift|RGB‑D SLAM|RTAB‑Map|C++ — RTAB‑Map, ROS 2|
|Understand what objects are|Geometry has no meaning|AI object detection|YOLO|Python (training) / C++ (runtime) — PyTorch, TensorRT|
|Run fast on edge hardware|Limited power & compute|Optimized inference|TensorRT|C++ — TensorRT|
|Turn understanding into motion|Robot must plan safely|Navigation & planning|ROS 2 Nav2|C++ — ROS 2 Nav2|

