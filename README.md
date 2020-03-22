# aubo_pick_put

pick and put based on the aubo arm.

## Install

1. 需要先安装realsensor_ros 驱动
2. 配置dope cfg，并使得输出位姿估计 tpoic 为 *“/dope/pose_soap“*
3. project已内配置 auco_ros，手眼标定包，手眼标定数据为手动发送，详见 ”maubo_pick_put.launch“ 文件注释。 且标定数据为当时安装数据，现安装数据可能会有改变。



## Run

```c++
roslaunch control maubo_pick_put.launch
```

*Notes:* 

1. 需先运行6D估计程序
2. launch中包含如下三个程序
   - 手眼标定数据发布

   - tf坐标转换，抓取数据预处理

   - 抓取程序

 3. 抓取控制基于moveit，可能需要事先安装moveit各类pkg

      



   

   