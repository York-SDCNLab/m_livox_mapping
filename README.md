# Modified_livox_mapping
This is a modified version of the [original livox_mapping](https://github.com/Livox-SDK/livox_mapping).
## Purposes of this Projecrt
* Make the original project able to run with ROS Noetic in Ubuntu 20.04.
* Collect a point cloud that contains multiple fiducial markers from a SLAM framework.
* Save the intensity values for the points of the final 3D map.
## Modifications
* Solved the conflicts between the old-version OpenCV and the OpenCV inside Noetic. (Cmake error will occur otherwise)
* Solved the display issue due to caused by different rviz versions. Now, even using Noetic, you can watch the mapping process without changing the settings in rviz.
* Added a new script to convert the format of the final-built 3D map from RGB8 to XYZI.
## How to use
``git clone https://github.com/York-SDCNLab/Modified_livox_mapping.git``


The rosbag is available [here](https://drive.google.com/file/d/1ZmS2tajLKvlstaqA8L-T6nzKj0bfL30n/view?usp=sharing).
