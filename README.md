# H2LID: a Handheld Hemispherical view LiDAR-IMU Dataset

## Introduction:
This is a LiDAR-IMU dataset using a handheld hemispherical view LiDAR-IMU system.

## Author:

## 1. COLLECTION PLATFORM

Our handheld system integrates a nine-axis IMU ([Owllmo IMU3910](http://www.owllmo.com/productinfo/341948.html)) and a hemispherical view LiDAR ([RoboSense RS-Bpearl](https://www.robosense.cn/en/rslidar/RS-Bpearl)). Two outdoor data sequences are collected in open-air environments by fixing the system on a mobile platform equipped with a GNSS+INS system, as shown below.

<div align=center>
	<img src="https://github.com/duanxz0127/H2LID/blob/main/mypics/platform.jpg" width="800px">
</div>
<p align=center>Figure 1. The equipment for outdoor data collection</p>


## 2. DATASET SEQUENCES

Sequence|Collection Date|Total Size|Duration|Rosbag|Ground Truth
--|:--|:--:|--:|--:|--:
Indoor 1|2022-01-16|3.8G|227s|[Rosbag]()|--
Indoor 2|2022-01-16|709M|11s|[Rosbag]()|--
Outdoor 1|2022-01-16|4.5G|331s|[Rosbag]()|--
Outdoor 2|2022-01-16|5.1G|341s|[Rosbag]()|--
Outdoor 3|2022-01-16|10.8G|953s|[Rosbag]()|[Ground Truth](https://whueducn-my.sharepoint.com/:t:/g/personal/2016302590017_whu_edu_cn/EWbAgaaGECZAvlvonh-3KccBlc70nYBGJOek62BAFnMMeA?e=cVGX3G)
Outdoor 4|2022-01-16|5.9G|567s|[Rosbag]()|[Ground Truth](https://whueducn-my.sharepoint.com/:t:/g/personal/2016302590017_whu_edu_cn/Ef5qaqZWDipHo64U0wCzAvgBZ_y0cfVyOrRC2cxDdUUPkQ?e=FJJtN1)

## 3. DATA FORMAT

For LiDAR data and IMU data, the rostopics of our rosbag sequences are listed as follows:

* LiDAR: `/horizontal_laser_3d` 
* IMU: `/imu` 

For Ground Truth (GNSS+INS), the basic information are:



* Datum: `WGS84`
* Master 1: `Name 744, Status ENABLED, Antenna height 0.090 m, to L1PC [Generic(NONE)], Lat, Lon, El Hgt 30 31 41.04001, 114 21 19.90145, 26.630 m [WGS84, N/A]`
* Remote: `Antenna height 0.000 m, to L1PC [Generic(NONE)]`
* IMU to GNSS Antenna Lever Arms: `x=-0.034, y=-0.283, z=0.342 m (x-right, y-fwd, z-up)`
* Body to Sensor Rotations: `xRot=90.000, yRot=0.000, zRot=-90.000 degrees (Rotate IMU into Vehicle Frame)`
* Map projection Info: `Defined grid: Gauss Kruger (3 deg), Zone 38`



The content of each column in the file and some sample data are listed as follows:

GPSTime(sec)|Easting(m)|Northing(m)|H-Ell(m)|Heading(deg)|Pitch(deg)|Roll(deg)|Latitude(deg)|Longitude(deg)|VEast(m/s)|VNorth(m/s)|VUp(m/s)|Q
--|:--|:--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:
9879.920|533843.632|3379901.251|17.899|-4.8583430063|0.7827190222|-0.0842668245|30.5388466765|114.3526809197|0.000|-0.002|-0.001|1
9879.925|533843.632|3379901.251|17.899|-4.8581697398|0.7827817133|-0.0844801964|30.5388466766|114.3526809197|0.000|-0.002|-0.001|1
9879.930|533843.632|3379901.251|17.899|-4.8580207716|0.7826683263|-0.0845637112|30.5388466766|114.3526809197|0.000|-0.002|-0.001|1
9879.935|533843.632|3379901.251|17.899|-4.8579476728|0.7827301471|-0.0845647536|30.5388466767|114.3526809196|0.000|-0.002|-0.001|1
9879.940|533843.632|3379901.251|17.899|-4.8579405575|0.7827763180|-0.0845550087|30.5388466767|114.3526809196|0.000|-0.002|-0.001|1
