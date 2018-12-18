-----------12/18/18------

ris_14570.world	--------	iris #4, for px4 sitl, port 14570
iris_2uav.world --------	2xiris, px4 sitl, port 14570, 14571

iris_cam2pole.world  -----	iris #2,3, px4 sitl, cam,fixed on pole, 14570 
iris_cam2.world     -----	iris #2,3, same as 2uav.world, with cam  
iris_cam.world      ----	iris #1, same as 14570.world, with cam

------------------- iris models----------------------------------
model #1 ---- iris_px4_standoff_demo_cam	---- imu, mavlink_interface 14560, gimbal_small_2d_px4
model #2 i--- iris_px4_standoff_demo_cam1	---- imu, mavlink_interface 14570, gimbal_small_2d_px4_1
model #3 ---- iris_px4_standoff_demo_cam2	---- imu, mavlink_interface 14571, gimbal_small_2d_px4_2a
model #4 ---- iris_px4_standoff_demo_1	--- imu, mavlink_interface 14570,

-------------------- gimbal_small_2d xxx------
gimbl with camera and plugin 

#1 gimbal_small_2d	------ gimbl plugin, camera without plugin
#2 gimbal_small_2d_px --- camera with ros_camera.so plugin, topic ardrone/image_raw, no gimbal plugin
#3 gimbal_small_2d_px_1 --- same as #2, topic ardrone1/image_raw
#4 gimbal_small_2d_px_2 --- same as #2, topic ardrone2/image_raw

