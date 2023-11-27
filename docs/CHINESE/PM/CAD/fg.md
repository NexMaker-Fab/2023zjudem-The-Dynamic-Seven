# **Pluging**

在Fusion 360中，插件（有时称为“加载项”）是一块软件，可扩展Core Fusion 360应用程序的功能。这些插件通常是由第三方开发人员或用户创建的，可以安装以提供Fusion 360中的其他功能，工具或功能。插件可用于简化特定的工作流程，添加新的设计或仿真工具，与外部软件或外部软件或集成硬件等等。

以下是Fusion 360插件的一些常见用途：

1. 自定义工具：插件可以添加根据特定需求量身定制的自定义设计，仿真或制造工具，而核心软件可能无法使用。

2. 文件导入/导出：插件可以支持用于导入或导出设计的各种文件格式，从而允许与其他软件进行互操作。

3. 自动化：插件可以自动化重复任务或创建自定义脚本以有效执行设计操作。

4. 数据管理：一些插件有助于数据管理，帮助用户更有效地组织和跟踪设计数据。

5. 集成：插件可以将Fusion 360与外部应用程序或硬件集成，从而增强其针对特定行业或流程的功能。

6. 仿真和分析：某些插件提供高级模拟和分析功能，例如有限元分析（FEA）或计算流体动力学（CFD）。

7. CAM（计算机辅助制造）：CAM插件可以直接从Fusion 360中生成用于CNC加工和其他制造过程的工具路径。

8. 渲染和可视化：插件可以提高渲染和可视化功能，从而使设计更现实。

   <br>
   <br>

## Planetary Gear Train Modeling
<br>
<br>


行星齿轮列车是一种机械系统，该机械系统由以特定配置为行星或epicyclic齿轮布置的齿轮组成。它包括三个主要组成部分：位于中心的太阳齿轮，围绕太阳齿轮旋转的行星齿轮以及封闭行星齿轮的环齿轮。这些齿轮以一种使它们能够以复杂但可预测的方式传输运动和扭矩的方式互连。

对行星齿轮训练进行建模涉及理解和数学代表其行为。工程师和数学家使用方程式和图表来描述齿轮之间的相互作用，速度比，扭矩传输和旋转方向在系统内的变化。

为了建模行星齿轮列车，通常会考虑每个齿轮上的牙齿数量，齿轮尺寸，旋转速度和齿轮布置等因素。从齿轮力学原理（例如齿轮和运动学定律）中得出的方程式用于预测和分析系统的性能。计算机模拟和数学模型有助于理解在不同条件和配置下齿轮列车的行为。

在各个领域，包括机械工程，汽车设计，机器人技术等，建模行星齿轮列车至关重要，因为它允许工程师预测性能，优化设计并确保机械和系统内的有效传动力传输。
<br>
<br>

**3D Model**

设置设计参数
该项目将建造一个包含三个齿轮的齿轮，即戒指，太阳和平面图。齿轮配给1：6，固定：环齿轮，驱动：太阳齿轮，输出：载体

打开Fusion 360应用程序。

在Fusion任务栏中选择实用程序。

<br>
<img src="PM/CAD/Plugin/figure1.png" > <br>
<br>
选择加载项，然后选择脚本和加载项选项（或单击“ shift + s”）。这将在屏幕上弹出脚本和附加框选项。
<br>
<img src="PM/CAD/Plugin/figure2.png" > <br>
<br>

单击“加载”选项，向下划掉并选择SpearGear选项，然后单击“运行”。此添加一个SpearGear命令在<b> create </b> pannel中。单击命令示例弹出窗口上的确定。
<br>
<img src="PM/CAD/Plugin/figure3.png" style="float: center;" width=700 > <br>
<br> <br>
单击Fusion Workplace上的固体，然后单击创建选项，然后在创建选项上选择SpearGear。
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
<br>

如下所示，设置Spur Gear参数，然后单击“确定”。这会产生带有80颗牙齿的刺激性，但我们想要倒数。
<br>
<img src="PM/CAD/Plugin/figure5.png" style="float: center;" width=700 > <br>
<br>

单击创建并选择圆柱体。选择任何平面，然后从圆的中心绘制气缸。
<br>
<img src="PM/CAD/Plugin/figure6.png" style="float: center;" width=700 > <br>
<br>
设置参数如下所示，然后单击确定
<br>
<img src="PM/CAD/Plugin/figure7.png" style="float: center;" width=700 > <br>
<br>
现在，我们将使用挤出命令从自行车运动机上切割齿轮的形状。激活自行车运动员
<br>
<img src="PM/CAD/Plugin/figure8.png" style="float: center;" width=700 > <br>
<br>
按E进行挤出。将距离设置为-10mm，然后选择矛齿轮作为配置文件和其他参数，如下所示。注意：配置文件选项；单击装备的脸以选择它
<br>
<img src="PM/CAD/Plugin/figure9.png" style="float: center;" width=700 > <br>
<br>
现在，选择矛枪（80TEETH）组件，然后右键单击Speargear（80Teeth）。选择删除选项，然后单击“确定”
<br>
<img src="PM/CAD/Plugin/figure10.png" style="float: center;" width=700 > <br>
双击组件2并将其重命名为环齿轮
<br>
<img src="PM/CAD/Plugin/figure11.png" style="float: center;" width=700 > <br>
现在让我们对行星进行建模。通过单击创建并选择矛齿轮选项来创建另一个超级射击。
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
设置参数，如下所示。其余参数将保持不变，除非牙齿的数量为32，而其他两个参数如下所示，然后单击“确定”
<br>
<img src="PM/CAD/Plugin/figure12.png" style="float: center;" width=700 > <br>
按键盘上的M移动组件，然后在移动/复制菜单中的Move Object Option上移动组件，然后在Origin中放大，以选择“为中心”作为选择选项。首先检查创建复制选项，然后将Y轴设置为48mm，目的是制作齿轮的副本。
<br>
<img src="PM/CAD/Plugin/figure13.png" style="float: center;" width=700 > <br>

再次按M，这次将旋转添加为运动类型，选择要为齿轮中心的轴，然后将角度设置为120度。首先检查创建复制选项。目的是制作另一个装备的副本
<br>
<img src="PM/CAD/Plugin/figure14.png" style="float: center;" width=700 > <br>

单击确定之前，请检查免费模式，然后将Y轴设置为48mm，然后单击确定
<br>
<img src="PM/CAD/Plugin/figure15.png" style="float: center;" width=700 > <br>
再次按M并添加旋转作为运动类型，选择为齿轮中心的轴，并将角度设置为240度。请勿检查复制选项，因为这是最后一个副本
<br>
<img src="PM/CAD/Plugin/figure16.png" style="float: center;" width=700 > <br>

单击确定之前，请检查免费模式，然后将Y轴设置为48mm，然后单击确定。 
<br>
<img src="PM/CAD/Plugin/figure17.png" style="float: center;" width=700 > <br>
现在，行星齿轮已经到位了。
通过单击创建并选择矛齿轮选项来创建另一个超级
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
设置参数，如下所示。其余参数将保持不变，除了16个牙齿的数量，然后单击确定
<br>
<img src="PM/CAD/Plugin/figure18.png" style="float: center;" width=700 > <br>
现在，太阳齿轮已经到位。
将16齿长矛齿轮设置为有效组件，然后单击草图
<br>
<img src="PM/CAD/Plugin/figure19.png" style="float: center;" width=700 > <br>

单击此齿轮的脸并选择捕获位置
<img src="PM/CAD/Plugin/figure20.png" style="float: center;" width=700 > <br>
然后按P进行项目。然后在当前草图上选择输入轴直径作为几何。单击确定，然后单击完成草图
<img src="PM/CAD/Plugin/figure21.png" style="float: center;" width=700 > <br>
按E排除E，然后选择该输入轴直径作为配置文件，将距离设置为-40mm，在操作选项上选择一个连接以加入轴
<img src="PM/CAD/Plugin/figure22.png" style="float: center;" width=700 > <br>
让我们将矛齿轮（32齿）重命名为行星齿轮和刺齿轮（16齿），因为太阳齿轮只是要组织起来
<img src="PM/CAD/Plugin/figure23.png" style="float: center;" width=700 > <br>
现在看一下草图的前 /顶 /后部 /底部视图，齿轮不是集体游行。
<img src="PM/CAD/Plugin/figure24.png" style="float: center;" width=700 > <br>
现在按M并选择旋转，然后选择要移动的组件，而轴是齿轮的中心，然后手动旋转齿轮的位置，直到它们正确匹配为止。对于其余的齿轮，请执行同样的操作，直到它们完全匹配为止。
<img src="PM/CAD/Plugin/figure25.png" style="float: center;" width=700 > <br>
一旦一切都正确匹配，请捕获位置
<img src="PM/CAD/Plugin/figure26.png" style="float: center;" width=700 > <br>

现在，最后一部分是将每个行星齿轮连接到输入轴的载体。
通过选择创建然后选择新组件来创建新组件
<img src="PM/CAD/Plugin/figure27.png" style="float: center;" width=700 > <br>
命名组件“载体”，然后单击“好”
<img src="PM/CAD/Plugin/figure28.png" style="float: center;" width=700 > <br>
通过单击草图创建一个新草图，然后将鼠标放在一个平面齿轮之一的脸上
<img src="PM/CAD/Plugin/figure29.png" style="float: center;" width=700 > <br>
单击P进行投影并选择齿轮的所有内径，如下所示，请单击“确定”
<img src="PM/CAD/Plugin/figure30.png" style="float: center;" width=700 > <br>
选择中心直径圆，并在所有齿轮中创建直径为10直径的圆。确保缩小齿轮的中心以将鼠标放置以进行绘制。
<img src="PM/CAD/Plugin/figure31.png" style="float: center;" width=700 > <br>
选择Aline加入所有齿轮。绘制连接所有齿轮的载体线
<img src="PM/CAD/Plugin/figure32.png" style="float: center;" width=700 > <br>
选择标记以确保线将线连接到圆上。选择几何图形，这是线条，每个点处的齿轮圆与线接触EG，如下所示
<img src="PM/CAD/Plugin/figure34.png" style="float: center;" width=700 > <br>
选择在交叉路口上指定半径的圆角。选择两行进行交集，然后单击确定并完成草图 
<img src="PM/CAD/Plugin/figure33.png" style="float: center;" width=700 > <br>
按E在键盘上排除。在配置文件上，选择齿轮的所有直径和轴的所有侧面（6组分），如下所示，并设置其他参数，如图所示
<img src="PM/CAD/Plugin/figure35.png" style="float: center;" width=700 > <br>
掩盖身体组件并揭示载体的草图组件，如下所示。按E再次排除。在配置文件上仅选择Plannet齿轮的直径和（3个内圆的Atotal），并设置其他参数，如图所示
<img src="PM/CAD/Plugin/figure36.png" style="float: center;" width=700 > <br>
揭示载体的身体成分和
按E再次排除。在配置文件上，仅选择Plannet齿轮的直径，（3个内圆的Atotal）设置参数如下所示，然后单击“确定”
<img src="PM/CAD/Plugin/figure37.png" style="float: center;" width=700 > <br>
揭开运营商的草图组件，然后单击草图，然后选择ATH载体作为平面
<img src="PM/CAD/Plugin/figure38.png" style="float: center;" width=700 > <br>

单击P进行项目，然后选择Sun Gear SA几何形状选项的中心
<img src="PM/CAD/Plugin/figure39.png" style="float: center;" width=700 > <br>
在太阳齿轮的中心创建直径为5mm的圆圈，然后单击“确定”并完成草图。
<img src="PM/CAD/Plugin/figure40.png" style="float: center;" width=700 > <br>

按E再次排除。在配置文件上，仅选择上面创建的太阳齿轮的直径，并设置其他参数，如图所示。此移动连接所有齿轮。注意：有时候，选择此内圆可能很难掩盖其他图层，例如身体，素描以选择此圆圈并在选择它之后将其放置。
<img src="PM/CAD/Plugin/figure41.png" style="float: center;" width=700 > <br>

现在，已经创建了载体连接到齿轮，现在模式已完成。
现在让我们定义关节。我们将用作构建关节，但首先让我们定义载体和每个平面图之间的关节。
选择组装并作为建筑联合选项
<img src="PM/CAD/Plugin/figure47.png" style="float: center;" width=700 > <br>
<br>
将参数设置为如下运动类型Revolute，首先选择“平面齿轮”，然后选择载体作为组件，然后选择“行星齿轮中心”作为快照（请记住要缩放中心）。
<img src="PM/CAD/Plugin/figure48.png" style="float: center;" width=700 > <br>
<br>
在其余的行星齿轮中重复此过程。注意：有时，很难选择平面齿轮和载体，尝试掩盖载体以选择行星齿轮组件并卸载载体并选择载体组件。
一开始，定义环齿轮已固定，现在让我们去戒指并选择地面以将其固定在适当的位置
<img src="PM/CAD/Plugin/figure49.png" style="float: center;" width=700 > <br>
<br>
现在，让我们定义托架和环齿轮，太阳和环齿轮之间的接头。
选择组装并选择作为建造接头，然后选择载体和环齿轮作为组件和中心为载齿轮的中心。对带环齿轮的载体和太阳齿轮重新修复，然后将连接命名为
<img src="PM/CAD/Plugin/figure50.png" style="float: center;" width=700 > <br>
<br>

让我们应用每个齿轮组件之间的运动链接。选择组装并选择运动链接
<img src="PM/CAD/Plugin/figure51.png" style="float: center;" width=700 > <br>
<br>
从关节菜单中创建一个在太阳环和载波环之间的运动链接，并设置其他参数，如下所示
<img src="PM/CAD/Plugin/figure52.png" style="float: center;" width=700 > <br>
<br>
在太阳齿轮和每个平面图之间建立一个运动链接。选择和选择运动链接。选择太阳环和平面载体。重复两个平面齿轮中其余的过程
<img src="PM/CAD/Plugin/figure53.png" style="float: center;" width=700 > <br>
<br>
当我们尝试旋转太阳齿轮时，现在看起来不好
<img src="PM/CAD/Plugin/figure54.png" style="float: center;" width=700 > <br>
<br>
重命名要组织的运动链接
<img src="PM/CAD/Plugin/figure55.png" style="float: center;" width=700 > <br>
<br>
现在编辑太阳和行星之间的运动链接
<img src="PM/CAD/Plugin/figure56.png" style="float: center;" width=700 > <br>
<br>
在太阳（首先选择）和平面链接之间设置关节的pameter，并在最后两个关节的齿轮齿轮的最后两个接头中重复使用，如下所示。现在，如果您旋转太阳装备，一切都正确匹配
<img src="PM/CAD/Plugin/figure57.png" style="float: center;" width=700 > <br>
<br>
该模型已经完成并且正在采取行动
<img src="PM/CAD/Plugin/figure59.png" style="float: center;" width=700 > <br>
<br>

<br>
<br>

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e530a2cd9cca71581?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

<br>
<br>

 <img style="float: center;" width=1280 height=600 src="PM/CAD/gear.gif">
        

<br>
<br>



## FM Gear
在这里，我们创建一个创建刺激齿轮。在这一部分中，我们使用插件来创建翼齿轮。

<img style="float: center;" width=1000 src="PM/CAD/fg/1st.jpg">

<br> 
首先，转到Fusion 360主界面，此页面到达。
<br><br>
<br> 

<img style="float: center;" width=700 src="PM/CAD/fg/2nd.jpg">
<br><br>
然后选择实用程序。
<br>
<br>

<img style="float: center;" width=700 src="PM/CAD/fg/3rd.jpg">
<br<br>>

然后转到“加载项”选项，然后选择“ Fusion 360 App Store”。

<br><br>
<img style="float: center;" width=700 src="PM/CAD/fg/4th.jpg">
<img style="float: center;" width=700 src="PM/CAD/fg/5th.jpg">
<br> <br>
然后，下载后才去搜索“ FM Gear”。安装后，FM齿轮插入选项出现在固体创建的FM齿轮中。
<br><br>
<img style="float: center;" width=700 src="PM/CAD/fg/6th.jpg">
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/7th.jpg">
<br>
现在我们可以看到该FM齿轮已到达。单击此处后，此页面到达。修复一切后，按OK，然后一齿轮到达。
<br>
<br>
<img style="float: center;" width=700 src="PM/CAD/fg/8th.jpg">

<br>
这是我们的一个装备。现在我们还添加一个装备。
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/9th.jpg">
 
<img style="float: center;" width=700 src="PM/CAD/fg/10.jpg">
<br>
 再次转到“固体”  - “创建”  - “ FM齿轮”. 
<br>
<img style="float: center;" width=700 src="PM/CAD/fg/12.jpg">
<br> <br> 然后单击“捕获位置”。
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/13.jpg">
<br>
然后这个接口到达。
<br<br>

<img style="float: center;" width=700 src="PM/CAD/fg/14.jpg">
<br> 还有“素描调色板”设置所有需要的东西，然后单击“完成草图”。
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/15.jpg">
<br>
<br>
然后再次转到“固体”，然后单击“创建”，然后选择“挤出”。
<img style="float: center;" width=700 src="PM/CAD/fg/16.jpg">
<br><br>
然后，此接口打开，选择所有内容后，单击“确定”。
<br> 
<img style="float: center;" width=700 src="PM/CAD/fg/17.jpg">
<br> 
稍后，选择“ Sketch1”。

<img style="float: center;" width=700 src="PM/CAD/fg/18.jpg">
<br><br>
然后转到“组装”，然后选择“关节”。
<img style="float: center;" width=700 src="PM/CAD/fg/19.jpg">
<br> 
<img style="float: center;" width=700 src="PM/CAD/fg/20.jpg">
<br><br>
当点击接头时，此接口会到达。然后设置“位置”和“运动”，然后单击“确定”。
<br<br>
<img style="float: center;" width=700 src="PM/CAD/fg/21.jpg">
<br>
再次转到“组装”，然后为大型装备选择“关节”。
<img style="float: center;" width=700 src="PM/CAD/fg/22.jpg">
<br<br> 
然后修复“位置”和“运动”。然后单击“确定”。

<br>
<img style="float: center;" width=700 src="PM/CAD/fg/23.jpg">
<img style="float: center;" width=700 src="PM/CAD/fg/24.jpg">
<br><br>
然后再次转到“组装”，然后选择“运动”，然后设置运动。
<br><br>

这是我们的项目。

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e6833968b711a1fe0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


<video width="700" height="500" controls>
  <source src="PM/CAD/fg/FMG.mp4" type="video/mp4">
  <source src="PM/CAD/fg/FMG.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>


