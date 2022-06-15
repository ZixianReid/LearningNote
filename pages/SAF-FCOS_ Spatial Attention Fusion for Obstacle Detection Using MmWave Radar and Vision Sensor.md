title:: SAF-FCOS: Spatial Attention Fusion for Obstacle Detection Using MmWave Radar and Vision Sensor

- ![image.png](../assets/image_1654583661233_0.png)
-
- 使用数据集： nuScenes
	- the nuScenes dataste is split as training dataset, validation dataset and test dataset,which have 700 scenes, 150 scenes and 150 scene
- 数据处理：
	- radar
		- 生成伪图像
			- ![image.png](../assets/image_1654584017786_0.png)
			- 根据上面的公式生成雷达图的中心点，生成以r为半径的圆为radar render
				- 根据生成的radar render进行过滤，
		-