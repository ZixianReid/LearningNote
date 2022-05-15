- ![Radar_and_vision_sensors_calibration_for_outdoor_3D_reconstruction.pdf](../assets/Radar_and_vision_sensors_calibration_for_outdoor_3D_reconstruction_1646570820869_0.pdf)
- Based on the inter-targets distance, Unlike DLT, do not need specific design to ensure that exact intersection of the target with the horizontal plane of the radar
- Calibration mathmatical
	- ![image.png](../assets/image_1646897703383_0.png)
	- keep three residuals minimize:
	  ![image.png](../assets/image_1646906254900_0.png)
	  ![image.png](../assets/image_1646906261385_0.png){:height 100, :width 472}
	  $x_2$ $y_2$ $z_2$ is the radar 3D location, r is radar depth and $\theta$ is the azimuth angle.
	  
	  radar points can be calcuated by
	  ![image.png](../assets/image_1646907963762_0.png)
	-
- Tip
	- New optimization residuals minimize way, improve the robustness of calibration approaches(do not need at the same horizon)
	- for 4D MMW, we should set target to different horizonal plan compared with radar plane to gain the elevation information.