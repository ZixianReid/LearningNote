title:: RVNet: Deep Sensor Fusion of Monocular Camera and Radar for Image-Based Obstacle Detection in Challenging Environments

- ![image.png](../assets/image_1653536952857_0.png)
-
- 融合类别：特征融合
-
- 识别网络：yolov3
-
- 数据特征处理
	- 雷达
		- 3D雷达点投影到image里，生成点图
		- 根据点图生成3通过伪图像（深度，侧向速读）
		-