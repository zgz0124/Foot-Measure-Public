# foot-measure

## 一、脚型测量项目概述：
> 简要流程图
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/目前工作.png" width="800px"></div>


## 二、项目背景：
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/项目背景.png" width="600px"></div>

> 优点
- 儿童选鞋：过往在零售门店，通常家长给孩子选购鞋子，会买稍微大一码或者半码的鞋子。不适脚的鞋容易造成高弓足、指甲受伤、拇趾外翻等。通过此系统获取足部3D模型，该知名鞋企可根据小朋友足部特点，推荐合适脚型和码数的鞋子，儿童健康鞋概念更深入人心。
- 鞋履定制：通过设备可快速采集足部3D数据，获取足部详尽的尺寸及形状参数，为鞋履定制提供可靠的数据支撑，比如儿童机能鞋定制、袜子定制、运动类鞋子定制，足膜定制，鞋楦定制等去打通制造端。
- 足部矫正：通过足部三维扫描获取足部3D数据，尺寸，足弓，足跟状态数据，足底受力区域等相关信息，可及时发现小朋友足部健康问题并及时干预，让孩子在最佳年龄阶段进行足部矫正。
- 专业导购：为门店提供数据支持，从消费者到店，脚型测量，到鞋子试穿，数据一目了然，通过专业脚型数据驱动业务增长，提升店内运营效率，个性化定制辅助营销，提高入店客人转化率。
- 虚拟展示：减少不同码数鞋的陈列空间，快速的新品试错，设备入店可增加科技感体验，逐步由传统面向库存生产的模式，转化为面向订单的柔性生产模式，提升业务与资金周转效率。


## 二、场景
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/设备.png" width="300px" height="250"></div>

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/设备图.png" width="300px" height="250"></div>

## 三、硬件设计
- 每个角度点云截取策略

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/硬件截取尺寸.png" width="1200px"></div>


## 四、标定过程
> 6相机一次性标定，实际现场图。
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/标定过程.png" width="500px"></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/标定模拟.png" width="900px"></div>

## 五、扫描点云

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/6视角.png" width="900px" height="130"></div>

## 六、后处理阶段

> 1、扫描点云
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-1扫描点云.png" width="400px" ></div>

> 2、标准模型
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-2、标准模型.png" width="400px" ></div>

> 3、点云配准
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-3、配准.png" width="400px" ></div>

> 4、配准结果
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-4、配准结果.png" width="400px" ></div>

> 5、坐标系显示
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-5、坐标系显示.png" width="400px" ></div>

> 6、点云统计滤波
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-5、点云统计滤波.png" width="400px" ></div>

> 7、法向计算及校准
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-7、点云法向计算.png" width="400px" ></div>

> 8、封装网格
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-8、封装点云.png" width="400px" ></div>

> 9、网格平滑
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/后处理-9、网格平滑.png" width="400px" ></div>



## 七、尺寸

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸提取示意.png" width="200px" ></div>

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸.png" width="400px" ></div>

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/脚类型.png" width="450px" ></div>

## 八、可视化
> 为了更好直观地查看尺寸提取效果，做了可视化地内容，将点云导入，点击计算就可以直观地看到特征点以及尺寸计算的结果。

> 脚印提取的可视化
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/有脚印11.jpg" width="430px" height="661" style="zoom:40%;" ></div> 

> 无脚印的尺寸提取可视化
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸11.jpg" width="430px" height="649" ></div> 
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/有脚印12.jpg" width="430px" height="268"></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸12.jpg" width="430px" height="793"></div>


## 八、输出格式
- 表格CSV
- PDF

## 九、用户报告
> 根据用户测量结果，输出相关报告

<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸1.png" width="700px" ></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸2.png" width="700px" ></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸3.png" width="700px" ></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸4.png" width="700px" ></div>
<div align=center><img src="https://github.com/Mr-ZhuJun/Foot-Measure-Public/blob/main/Reference/尺寸5.png" width="700px" ></div>

