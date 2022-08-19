# H2LID: a Handheld Hemispherical view LiDAR-IMU Dataset

## Introduction:
This is a LiDAR-IMU dataset using a handheld hemispherical view LiDAR-IMU system.

## Author:

## 1. COLLECTION PLATFORM
Our handheld system integrates a nine-axis IMU ([Owllmo IMU3910](http://www.owllmo.com/productinfo/341948.html)) and a hemispherical view LiDAR ([RoboSense RS-Bpearl](https://www.robosense.cn/en/rslidar/RS-Bpearl)). Two outdoor data sequences are collected in open-air environments by fixing the system on a mobile platform equipped with a GNSS + Inertial Navigation System (INS) system, as shown below.

<div align=center>
	<img src="https://github.com/duanxz0127/H2LID/blob/main/mypics/platform.jpg" width="1000px">
</div>
<p align=center>Figure 1. The equipment for outdoor data collection</p>


## 2. DATASET SEQUENCES

Sequence|Collection Date|Total Size|Duration|Rosbag|GT
--|:--|:--:|--:|--:|--:
Indoor 1|2022-01-16|3.8G|227s|[Rosbag]()|--
Indoor 2|2022-01-16|709M|11s|[Rosbag](https://whueducn-my.sharepoint.com/:f:/g/personal/2016302590017_whu_edu_cn/ElZp81OzPQxHpWypy7iXwXYBkiv5_yBZRCi4UqVcLaW8NQ?e=mGMJf8)|--
Outdoor 1|2022-01-16|4.5G|331s|[Rosbag]()|--
Outdoor 2|2022-01-16|5.1G|341s|[Rosbag]()|--
Outdoor 3|2022-01-16|10.8G|953s|[Rosbag]()|[GT](https://whueducn-my.sharepoint.com/:t:/g/personal/2016302590017_whu_edu_cn/EWbAgaaGECZAvlvonh-3KccBlc70nYBGJOek62BAFnMMeA?e=cVGX3G)
Outdoor 4|2022-01-16|5.9G|567s|[Rosbag]()|[GT](https://whueducn-my.sharepoint.com/:t:/g/personal/2016302590017_whu_edu_cn/Ef5qaqZWDipHo64U0wCzAvgBZ_y0cfVyOrRC2cxDdUUPkQ?e=FJJtN1)
