

## 什么是 3D 打印？

3D打印，也称为增材制造，是基于数字模型通过逐层添加材料来创建三维物体的过程。该工艺可以生产复杂的形状和结构，而通过传统的制造方法可能很难或不可能实现这些形状和结构。

3D 打印技术有多种类型，每种技术都有其原理和变体。一些常用的 3D 打印技术包括：

**熔融沉积成型 (FDM) / 熔丝制造 (FFF)：** FDM 是最流行的 3D 打印方法之一。它涉及通过喷嘴逐层加热和挤出热塑性长丝以形成物体。

**立体光刻 (SLA)：** SLA 使用一桶由紫外激光固化的液体树脂来创建层并固化树脂，形成所需的物体。

**选择性激光烧结 (SLS)：** SLS 采用高功率激光逐层烧结粉末材料，例如塑料、金属或陶瓷，使颗粒融合以形成最终物体。

**数字光处理 (DLP)：** 与 SLA 类似，DLP 使用光源（通常是投影仪）逐层固化树脂以形成物体。

**选择性激光熔化 (SLM) / 直接金属激光烧结 (DMLS)：** 这些技术使用高功率激光将金属粉末逐层熔化和熔合在一起，以制造金属物体。

**粘合剂喷射：** 粘合剂喷射涉及将粘合剂选择性地沉积到粉末材料床上。一旦一层完成，就会铺开一层新的粉末，重复这个过程直到物体形成。

**材料喷射：** 材料喷射的操作方式与喷墨打印类似，其中材料液滴选择性地沉积到构建平台上并固化或凝固以形成物体。

这些是一些主要的 3D 打印技术，每种技术都有自己的优势、局限性以及在航空航天、汽车和医疗保健等各个行业的特定应用。

## 3D打印机实验

＃＃＃ 软件

* Fusion360
* FlashPrint 5
  
### 如何从 Fusion360 转换 **STL** 文件

<br>
<img style="float: center;" width=700 src="PM\3D_print\f.png">
<br>
<br>
<img style="float: center;" width=700 src="PM\3D_print\f_1.png">
<br>
<br>
<img style="float: center;" width=700 src="PM\3D_print\f_3.png">
<br>

现在在 FlashPrint 软件中打开 STL 文件。


＃＃＃ 用户指南

#### 1.软件介绍

FDM技术切片软件Flashforge FlashPrint 5全新改版升级。通过全新的界面设计和功能优化，操作简单便捷。只需点击几下即可准备好切片文件，操作快速、高效、流畅。
<br>


#### 2.软件安装

Download the latest version of [FlashPrint 5](https://www.flashforge.com/product-detail/FlashPrint-slicer-for-flashforge-fdm-3d-printers)

<br>
#### 3.软件操作

当我们第一次打开软件时，我们需要修复机器类型。
<br>

<img style="float: center;" width=700 src="PM\3D_print\1.png">
<br>

<img style="float: center;" width=700 src="PM\3D_print\2.png">

<br>我们选择“Guider II S Series”，然后按“确定”。

<br><br>
<img style="float: center;" width=700 src="PM\3D_print\3.png"><br>

现在，转到“文件”，选择“加载”，然后上传我们要打印的文件。

<br>

<img style="float: center;" width=700 src="PM\3D_print\4.png">
<br>

单击“加载”后，选择文件并按“打开”。
<br><br>

<img style="float: center;" width=700 src="PM\3D_print\5.png"><br>
现在，“埃菲尔铁塔”项目在界面框中可见。
<br>

<img style="float: center;" width=700 src="PM\3D_print\6.png">
<br>
从不同角度查看模型。
<br>

<img style="float: center;" width=700 src="PM\3D_print\7.png">
<br>
单击它可以沿X、Y轴移动模型；按住Shift+鼠标，单击可沿Z轴移动。在这里，始终尝试选择“On Platform”。
<br>

<img style="float: center;" width=700 src="PM\3D_print\8.png">
<br>
旋转模型。
<br>

<img style="float: center;" width=700 src="PM\3D_print\9.png">
<br>
缩放模型尺寸。这里我们可以选择点“统一缩放”或“英寸”。对于我们的项目，我们选择了第一个。
<br>

<img style="float: center;" width=700 src="PM\3D_print\10.png">
<br>
从不同方向切割模型。
<br>

<img style="float: center;" width=700 src="PM\3D_print\11.png">
<br>
复制选定的模型文件。这里我们可以增加重复的数量，然后点击“确定”。 
<br>

<img style="float: center;" width=700 src="PM\3D_print\12.png">
<br>
这里最重要的是我们不能立即设置模型。如果我们将其从盒子中取出，则会出现红色框并通知出现问题并修复它然后打印。

<br>

<img style="float: center;" width=700 src="PM\3D_print\13.png">
<br>
如果我们一次放置两个以上的模型，那么我们需要检查它。自动布局部分。
<br>

<img style="float: center;" width=700 src="PM\3D_print\14.png">
<br>
进入支持编辑模式。
<br>
PM\3D_print\
<img style="float: center;" width=700 src="PM\3D_print\15.png">
<br>
这是一种选择，但打印后很难去除。
<br>

<img style="float: center;" width=700 src="PM\3D_print\16.png">
<br>
对于我们的模型，我们使用这个支撑，对于支撑柱尺寸，我们设置 1.5mm，因为这样我们在打印后很容易将其移除。
<br>

<img style="float: center;" width=700 src="PM\3D_print\17.png">
<br>
我们也可以手动完成。
<br>

<img style="float: center;" width=700 src="PM\3D_print\18.png">
<br>
进入擦塔编辑模式。
<br>

<img style="float: center;" width=700 src="PM\3D_print\19.png">
<br>
输入多机器控制接口。
<br>

<img style="float: center;" width=700 src="PM\3D_print\20.png">
<br>
进入机器连接界面。
<br>

<img style="float: center;" width=700 src="PM\3D_print\21.png">
<br>
现在按“开始切片”。首先，如我们所见，基本界面如下所示。
<br>

<img style="float: center;" width=700 src="PM\3D_print\22.png">
<br>

这是切片部分的基本模式。
<br>

<img style="float: center;" width=700 src="PM\3D_print\23.png">
<br>


现在进入专家模式。
<br>

<img style="float: center;" width=700 src="PM\3D_print\24.png">
<br>
在专家模式下，我们需要修复所有必需的事情。<br>

<img style="float: center;" width=700 src="PM\3D_print\25.png">
<br>

完成每个部分后，我们将单击“切片”。<br>

<img style="float: center;" width=700 src="PM\3D_print\26.png">
<br>
切片过程中。
<br>

<img style="float: center;" width=700 src="PM\3D_print\27.png">
<br>
当我们按下“切片预览”时，出现如下界面。
<br>
<img style="float: center;" width=700 src="PM\3D_print\30.png">
<br>

<video width="700" height="500" controls>
<source src="PM\3D_print\ef_video.mp4" type="video/mp4">
<source src="PM\3D_print\ef_video.ogg" type="video/ogg">
</video>

这是其中的一个视频。
<br><br>

<img style="float: center;" width=700 src="PM\3D_print\28.png">
<br>
这是下载选项我们可以将其下载到闪存驱动器，然后我们可以打印它。
<br>
<img style="float: center;" width=700 src="PM\3D_print\29.png">
<br>
我们直接将其发送到打印机，但在我们的例子中，我们使用闪存驱动器在打印机中输入输出程序。

## Setup on FlashPrint 5

打开机器
<img src="PM\3D_print\machine_on.jpg" style="float: center;" width=800 height=700 >
<br>

我可以看到界面。
<br>
<img src="PM\3D_print\build.jpg" style="float: center;" width=800 height=700 >
<br>

点击“工具”即可看到该功能。
<br>
<img src="PM\3D_print\interface.jpg" style="float: center;" width=800 height=700 >
<br>

**“灯丝”**在此部分用户可以加载和卸载灯丝。
<br>
<img src="PM\3D_print\pla.jpg" style="float: center;" width=800 height=700 >
<br>

对于我们的机器，我们使用这种灯丝。
<br>
<img src="PM\3D_print\filament_t.jpg" style="float: center;" width=800 height=700 >
<br>

* Print temperature 220-240c
* Bed temperature 100c

**灯丝加载程序**
在 FlashPrint 软件中查找标有“加载”的选项或图标。该选项通常位于菜单或软件界面的主屏幕上。
<br>
<img src="PM\3D_print\load_f.png" style="float: center;" width=800 height=700 >
<br>

* 单击“加载”。 FlashPrint 将引导您逐步完成耗材加载过程。
* 它可能会要求您将喷嘴预热到适合您所使用的灯丝的温度。
* 喷嘴加热后，系统会提示您手动将耗材送入挤出机。可能有一个杠杆或释放机制，可以更轻松地插入灯丝。
* 将耗材送入挤出机，直到感觉到它抓住耗材并开始从喷嘴中挤出。确保它顺利、均匀地出来。

<br>
<img src="PM\3D_print\f_n.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_9.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\filament_load.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_8.jpg" style="float: center;" width=800 height=700 >
<br>



**灯丝卸载程序：**

<br>
<img src="PM\3D_print\u_1.jpg" style="float: center;" width=800 height=700 >
<br>

* 在 FlashPrint 软件中查找标有“卸载”的选项或图标。该选项位于软件界面的主屏幕上。
* 在 FlashPrint 中启动耗材卸载过程后，软件可能会提示您执行手动步骤。
* 通常，您会被要求协助按下挤出机上的释放杆或按钮，同时轻轻拉出灯丝。
* 按照屏幕上的说明释放灯丝上的张力，并小心地将其从挤出机组件中取出。

<br>
<img src="PM\3D_print\interface.jpg" style="float: center;" width=800 height=700 >
<br>

**点击“级别”**

* FlashPrint 将指导您完成一系列调整打印机构建平台上的调平螺钉或旋钮的动作。
* 进行调整时，可能会要求您在喷嘴和打印床之间使用一张纸或调平卡。
* 目标是喷嘴和床之间达到理想的距离，确保纸张/卡片可以在轻微阻力下移动，而不会太松或太紧。
<br>
<img src="PM\3D_print\l_3.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_1.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_5.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_6.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_4.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_2.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\l_7.jpg" style="float: center;" width=800 height=700 >
<br>

现在连接 USB 驱动器
<br>
<img src="PM\3D_print\pendrive.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\usb.jpg" style="float: center;" width=800 height=700 >
<br>

从这里选择您的 3D 模型。

<video width="720" height="540" controls>
<source src="PM\3D_print\m_1.mp4" type="video/mp4">
<source src="PM\3D_print\m_1.ogg" type="video/ogg">
您的浏览器不支持视频标签。

</video>

<br>

<br>
<img src="PM\3D_print\m_1.jpg" style="float: center;" width=800 height=700 >
<br>
<br>



**WORKING TIME**
<br>
<img src="PM\3D_print\on__mm.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\on_p.jpg" style="float: center;" width=800 height=700 >
<br>
<br>
<img src="PM\3D_print\r_p.jpg" style="float: center;" width=800 height=700 >
<br>
清洁模型后
<br>
<img src="PM\3D_print\output.jpg" style="float: center;" width=800 height=700 >
<br>

<video width="720" height="540" controls>
<source src="PM\3D_print\final.mp4" type="video/mp4">
<source src="PM\3D_print\final.ogg" type="video/ogg">
您的浏览器不支持视频标签。
</video>

<br>
<br>



# 组装多零件3D模型

<br>
<br>

<video width="720" height="540" controls>
<source src="PM\3D_print\fusion.mkv" type="video/mp4">
<source src="PM\3D_print\final.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
<br>

<video width="720" height="540" controls>
<source src="PM\3D_print\flshprint.mkv" type="video/mp4">
<source src="PM\3D_print\final.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>

<br>

<img src="PM\3D_print\slider_1.jpg" style="float: center;" width=800 height=700 >
<br>
<br>

<img src="PM\3D_print\silder_2.jpg" style="float: center;" width=800 height=700 >
<br>

<br>

<br>

# G 代码

* G代码是一种用于CNC（计算机数控）机器的编程语言。 G代码代表“几何代码”。
* 这种语言告诉机器要做什么或如何做某事。 G 代码命令指示机器向何处移动、移动的速度以及遵循的路径。
* G 代码命令指示机器沉积材料，一层又一层形成精确的几何形状。

## 通用 G 代码命令

### G00 – 快速定位

* G00 指令使机床以最大移动速度从当前位置移动到指定点或指令指定的坐标。

<img src="PM\3D_print\g00.webp" style="float: center;" width=700 >
<br>

* G00 是非切割运动，其目的是快速将机器移动到所需位置以开始某种作业，例如切割或打印。
*

### G01 – 线性插补

G01 G代码指令指示机床以设定的进给率或速度沿直线移动。我们使用 X、Y 和 Z 值指定结束位置，并使用 F 值指定速度。
<br>
<img src="PM\3D_print\g01.webp" style="float: center;" width=700 >
<br>
与仅用于定位的 G00 指令不同，G01 指令在机床执行主要作业时使用。如果是车床或铣床，则直线切割材料；如果是 3D 打印机，则直线挤压材料。

## G02 – 顺时针圆弧插补

G02指令告诉机器以顺时针方向做圆周运动。除了终点参数之外，这里我们还需要定义旋转中心，或者说圆弧起点到圆弧中心点的距离。起点实际上是上一个命令的终点或当前点。
<br>
<img src="PM\3D_print\g02.webp" style="float: center;" width=700 >
<br>
在上例中，G01 指令将机床移动到 X5、Y12 点。现在这将是 G02 命令的起点。 G02指令的X、Y参数设定终点。现在，为了使用圆周运动或使用圆弧到达终点，我们需要定义其中心点。我们使用 I 和 J 参数来做到这一点。 I 和 J 的值相对于前一个命令的起点或终点。因此，为了获得 X5 和 Y7 的中心点，我们需要沿 X 轴偏移 0，沿 Y 轴偏移 -5。

## G03 – 逆时针圆弧插补

与 G02 一样，G03 G 代码指令定义机床以圆弧模式移动。这里唯一的区别是运动是逆时针的。所有其他功能和规则与 G02 指令相同。
## G20/ G21 – 单位选择

G20 和 G21 命令定义 G 代码单位，英寸或毫米。

* G20 = 英寸
* G21 = 毫米
单位必须在程序开始时设置。如果我们不指定单位，机器将考虑前一个程序设置的默认单位。

## G17/ G18/ G18 – G代码平面选择

通过这些 G 代码命令，我们选择机器的工作平面。

* G17 – XY 平面
* G18 – XZ平面
* G19 – YZ平面
G17 是大多数 CNC 机床的默认设置。

## G28 – 回家

G28指令告诉机器将刀具移动到参考点或起始位置

## G90/ G91 – 定位G代码指令

G90 和 G91 命令告诉机器如何解释坐标。 G90 为绝对模式，G91 为相对模式。

* 在绝对模式下，刀具的定位始终从绝对点或零开始。因此，无论之前的位置如何，命令 G01 X10 Y5 都会将刀具带到该精确点 (10,5)。
* 另一方面，在相对模式下，刀具的定位是相对于最后一点的。因此，如果机床当前位于点(10,10)，则命令 G01 X10 Y5 会将刀具带到点(20,15)。该模式也称为“增量模式”。

## 更多命令和规则

因此，上面解释的 G 代码命令是最常见的命令，但还有更多。有刀具补偿、缩放、工作坐标系等命令。

除了 G 代码之外，还有在生成真正的成熟 G 代码程序时使用的 M 代码命令。以下是一些常见的 M 代码命令：

* M00 – 程序停止
* M02 – 程序结束
* M03 – 主轴开启 – 顺时针
* M04 – 主轴开启 – 逆时针
* M05 – 主轴停止
* M06 – 换刀
* M08 – 洪水冷却液开启
* M09 – 洪水冷却液关闭
* M30 – 程序结束

如果是 3D 打印机：

* M104 – 启动挤出机加热
* M109 – 等待挤出机达到 T0
* M140 – 启动床加热
* M190 – 等到床到达T0
* M106 – 设置风扇速度

其中一些命令需要适当的参数。例如，用M03打开主轴时，我们可以使用S参数来设置主轴转速。因此，M30 S1000 生产线将以 1000 RPM 的速度启动主轴。

＃＃＃ 参考

[G-code](https://howtomechatronics.com/tutorials/g-code-explained-list-of-most-important-g-code-commands/)
