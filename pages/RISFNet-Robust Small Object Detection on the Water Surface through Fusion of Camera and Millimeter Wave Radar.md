- ![Cheng-Robust Small Object Detection on the Water Surface thr.pdf](../assets/Cheng-Robust_Small_Object_Detection_on_the_Water_Surface_thr_1653275840195_0.pdf)
- ![image.png](../assets/image_1653275995198_0.png)
- 数据源：3D radar points cloud 和 RGB images
- 数据处理部分：
	- 雷达：
		- 1 ：采用pseudo image方式，文章称为 radar point density map
			- 伪图像三通道分别为
				- ![image.png](../assets/image_1653277346065_0.png)
				  r 为位置的平方和，v为速度，p为RCS
				-
		- 2：为解决单frame雷达点数过少问题，采用前面部分帧的雷达数据合成为一帧。
			- ![image.png](../assets/image_1653277599281_0.png)
			- 思考：是否采用该frame的前后几frame，而不是后frame效果会更好
			  background-color:: #793e3e
		- 3 使用VGG-13 backbone提取特征，然后使用Self-Attention Block增加真实的目标点减少噪声
	- 图像：
		- 使用CSPdarknet53提取特征