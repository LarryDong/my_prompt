# my_prompt
记录一些自己常用到的prompt。

## 读取csv绘制IMU数据
编写一个matlab代码，读取并绘制一个IMU文件的数据。IMU文件名为："/my_folder/imu.csv"，共N行7列，第一行是header，跳过不读取；每列依此是：时间戳（单位s）, ax, ay, az（单位：m/s2）, wx, wy, wz（单位：rad/s），由逗号分隔符分开。

绘制一个figure，包含两个子图，分别包括加速度和角速度的三轴数据，颜色xyz分别为rgb。横轴是时间戳，用实际物理时间。

## 读取rosbag绘制IMU数据。
编写一个matlab代码，读取一个rosbag并绘制其中的IMU数据。

rosbag名称为："my_rosbag.bag"，其中IMU数据格式为ros标准的sensor_msg::IMU，topic名称为："/ouster/imu"。加速度单位是m/s2，角速度单位是rad/s。

绘制一个figure，包含两个子图，分别包括加速度和角速度的三轴数据，颜色xyz分别为rgb。横轴是时间戳，第一个IMU的时间戳设置为0，之后按照物理时间绘制。
