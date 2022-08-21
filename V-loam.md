# V-loam

**<font color='red'>1.针对问题</font>**

**<font color='red'>2.主要贡献</font>**

**<font color='red'>3.解决方法</font>**

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**









# CamVox: A Low-cost and Accurate Lidar-assisted Visual SLAM System（2021）基于orbslam2



**<font color='red'>1.针对问题</font>**

​			**视觉结合lidar提高定位精度**

**<font color='red'>2.主要贡献</font>**

 -  ​	lidar和相机自动外部校准

- ​	更高的准确性和鲁棒性

![image-20220730204610040](/home/p/.config/Typora/typora-user-images/image-20220730204610040.png)

**<font color='red'>3.解决方法</font>**

​			激光雷达获取的点云经过imu校准后投影到深度图像然后将 RGB 图像与深度图像组合作为 RGBD 帧的输出，其中两个图像被格式化为相同大小并且像素级对应，（采用RGBD相机？？应该是）

​			接下来主要是校准，感觉创新点在这一部分

​			自己的数据集上测试 和VINS-mono livox horizon loam对比			

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**





# Direct Visual SLAM using Sparse Depth for Camera-LiDAR System（2018）



**<font color='red'>1.针对问题</font>**

- ​		深度增强的视觉里程计（与DEMO相近）使用直接法 单目相机和lidar稀疏信息结合

**<font color='red'>2.主要贡献</font>**

- ​		稀疏深度信息可用时直接法，不用提取特征来应对稀疏性

- ​		滑动窗口优化解决传感器视野限制。位姿图优化时，严格边缘化滑动窗口的位姿
- ​        关键帧



![image-20220730212002292](/home/p/.config/Typora/typora-user-images/image-20220730212002292.png)

**<font color='red'>3.解决方法</font>**

​			Tracking直接法，滑动窗口优化

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**



# DEMO Real-time Depth Enhanced Monocular Odometry（2014）

**<font color='red'>1.针对问题</font>**

视觉里程计可以通过深度信息（例如由 RGB-D 相机或与相机相关的激光雷达提供）来增强。然而，这种深度信息可能会受到传感器的限制，从而在视觉图像中留下无法获得深度的大面积区域。



**<font color='red'>2.主要贡献</font>**

使用激光雷达的点云深度值和三角测量所得的深度值为视觉特征点提供深度信息，可以提供更高精度的位姿估计和更高质量的地图

![image-20220820210536617](/home/p/.config/Typora/typora-user-images/image-20220820210536617.png)

**<font color='red'>3.解决方法</font>**

- 特征点和深度关联

​						深度信息存放在KD树中，找到离该特征点最近的三个点，构成平面将特征点投影构成的平面上得到特征点的深度。

- 两帧之间的运动估计

  ​			![image-20220820210953923](/home/p/.config/Typora/typora-user-images/image-20220820210953923.png)

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**

















# Lidar-Monocular Visual Odometry using Point and Line Features（2020）

**<font color='red'>1.针对问题</font>** 

​	定位精度？

**<font color='red'>2.主要贡献</font>**

**<font color='red'>3.解决方法</font>**

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**

**<font color='red'>1.针对问题</font>**

**<font color='red'>2.主要贡献</font>**

**<font color='red'>3.解决方法</font>**

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**

**<font color='red'>1.针对问题</font>**

**<font color='red'>2.主要贡献</font>**

**<font color='red'>3.解决方法</font>**

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**

**<font color='red'>1.针对问题</font>**

**<font color='red'>2.主要贡献</font>**

**<font color='red'>3.解决方法</font>**

**<font color='red'>4.不足之处</font>**

**<font color='red'>5.个人想法</font>**

