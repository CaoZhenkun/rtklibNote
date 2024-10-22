# RTKLIB
- [RTKLIB](#rtklib)
  - [数据获取](#数据获取)
    - [RTKGet](#rtkget)
  - [后处理](#后处理)
    - [RTKLIB界面程序](#rtklib界面程序)
    - [命令行程序](#命令行程序)

## 数据获取
### RTKGet
![alt text](image-2.png)
- 点击"?"进行时间转换

  ![点击"?"查看时间](image-3.png)

- OBS观测值文件

  下载地址2(http://www.igs.gnsswhu.cn/index.php)

  下载地址1(https://cddis.nasa.gov/archive/gnss/data/daily/2024/133/)

  o,d压缩方式不同

  ![alt text](image-4.png)

- NAV导航电文

  下载地址(https://cddis.nasa.gov/archive/gnss/data/daily/2024/092/24n/)

- EPH精密轨道
- CLK精密钟差
- ATK天线文件






## 后处理
### RTKLIB界面程序

视频教程(https://space.bilibili.com/479790048)

RTKLIB界面程序中后处理为rtkpost，其功能为后处理定位解算，传入观测文件、星历文件和其它改正信息文件，设置好解算选项进行后处理解算。

RTKPOST输入的是标准的 RINEX2.10,2.11,2.12,3.003.01,3.02 观测数据，
(GPS,GLONASS,Galileo,QZSS,BeiDou and  SBAS)导航电文文件，可以进行各种模
式的定位分析，主要包括有单点定位、DGPS/DGNSS、静态的、动态的、精密单点
静态和精密单点动态定位

1. 打开rtkpost

    ![alt text](image.png)
2. 输入 RINEX 流动站的观测数据路径点击...

   如果是相对定位模式，还要输入基准值接收机观测数据

   ʺSolutionʺ设置输出文件路径

3. 点击 Options,进行处理参数设置

   ![alt text](image-1.png)
4. 点击“Execute”开始数据分析计算

   当出现“done”表示处理完成

   处理过程中要停止，点击"Abort"

5. 处理完成后点击"view"可以查看数据

6. 点击 可以打开 RTKPLOT，点击 打开文档

### 命令行程序
命令行程序中为rnx2rtkp。
