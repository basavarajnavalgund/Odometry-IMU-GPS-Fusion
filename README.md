## Odometry, IMU, GPS fusion

 
 
#### Original repositories i have downloaded the code from
  
	robot_localization


#### Description
  
Filtered using:
1- EKF
2- UKF

Input: Odometry, IMU, and GPS (.bag file)

Output:
1- Filtered path trajectory
2- Filtered latitude, longitude, and altitude

It runs 3 nodes:
1- An *kf instance that fuses Odometry and IMU, and outputs state estimate approximations
2- A second *kf instance that fuses the same data with GPS
3- An instance navsat_transform_node, it takes GPS data and produces pose data

Also compared memory consumption of EKF and UKF nodes via htop

#### Please refer folder for results
