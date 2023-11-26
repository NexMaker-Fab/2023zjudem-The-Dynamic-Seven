
### Plugin
设置设计参数
该项目将建造一个包含三个齿轮的齿轮，即戒指，太阳和平面图。齿轮配给1：6，固定：环齿轮，驱动：太阳齿轮，输出：载体

打开Fusion 360应用程序。

在Fusion任务栏中选择实用程序。
<br>
<img src="PM/CAD/Plugin/figure1.png" >
<br>
选择加载项，然后选择脚本和加载项选项（或单击“ shift + s”）。这将在屏幕上弹出脚本和附加框选项。
<br>
<img src="PM/CAD/Plugin/figure2.png" >
<br>

单击“加载”选项，向下划掉并选择SpearGear选项，然后单击“运行”。此添加一个SpearGear命令在  create  pannel中。单击命令示例弹出窗口上的确定。
<br>
<img src="PM/CAD/Plugin/figure3.png" style="float: center;" width=700 >
<br>
单击Fusion Workplace上的固体，然后单击创建选项，然后在创建选项上选择SpearGear。
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 >
<br>

如下所示，设置Spur Gear参数，然后单击“确定”。这会产生带有80颗牙齿的刺激性，但我们想要倒数。
<br>
<img src="PM/CAD/Plugin/figure5.png" style="float: center;" width=700 >
<br>

单击创建并选择圆柱体。选择任何平面，然后从圆的中心绘制气缸。
<br>
<img src="PM/CAD/Plugin/figure6.png" style="float: center;" width=700 >
<br>
设置参数如下所示，然后单击确定.
<br>
<img src="PM/CAD/Plugin/figure7.png" style="float: center;" width=700 >
<br>
现在，我们将使用挤出命令从自行车运动机上切割齿轮的形状。激活自行车运动员 
<br>
<img src="PM/CAD/Plugin/figure8.png" style="float: center;" width=700 >
<br>
按E进行挤出。将距离设置为-10mm，然后选择矛齿轮作为配置文件和其他参数，如下所示。注意：配置文件选项；单击装备的脸以选择它
<br>
<img src="PM/CAD/Plugin/figure9.png" style="float: center;" width=700 >
<br>
现在，选择矛枪（80TEETH）组件，然后右键单击Speargear（80Teeth）。选择删除选项，然后单击“确定”
<br>
<img src="PM/CAD/Plugin/figure10.png" style="float: center;" width=700 >
双击组件2并将其重命名为环齿轮
<br>
<img src="PM/CAD/Plugin/figure11.png" style="float: center;" width=700 >
现在让我们对行星进行建模。通过单击创建并选择矛齿轮选项来创建另一个超级.
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 >
设置参数，如下所示。其余参数将保持不变，除非牙齿的数量为32，而其他两个参数如下所示，然后单击“确定”
<br>
<img src="PM/CAD/Plugin/figure12.png" style="float: center;" width=700 >
按键盘上的 M 移动组件，然后在移动/复制菜单中的Move Object Option上移动组件，然后在Origin中放大，以选择“为中心”作为选择选项。首先检查创建复制选项，然后将Y轴设置为48mm，目的是制作齿轮的副本。
<br>
<img src="PM/CAD/Plugin/figure13.png" style="float: center;" width=700 >

再次按 M，这次将旋转添加为运动类型，选择要为齿轮中心的轴，然后将角度设置为120度。首先检查创建复制选项。目的是制作另一个装备的副本
<br>
<img src="PM/CAD/Plugin/figure14.png" style="float: center;" width=700 >

单击确定之前，请检查免费模式，然后将Y轴设置为48mm，然后单击确定
<br>
<img src="PM/CAD/Plugin/figure15.png" style="float: center;" width=700 >
再次按M并添加旋转作为运动类型，选择为齿轮中心的轴，并将角度设置为240度。请勿检查复制选项，因为这是最后一个副本
<br>
<img src="PM/CAD/Plugin/figure16.png" style="float: center;" width=700 >

单击确定之前，请检查免费模式，然后将Y轴设置为48mm，然后单击确定。
<br>
<img src="fPM/CAD/Plugin/igure17.png" style="float: center;" width=700 >
现在，行星齿轮已经到位了。
通过单击创建并选择矛齿轮选项来创建另一个超级
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > 
<br>
设置参数，如下所示。其余参数将保持不变，除了16个牙齿的数量，然后单击确定
<br>
<img src="PM/CAD/Plugin/figure18.png" style="float: center;" width=700 > 
<br>
现在，太阳齿轮已经到位。
将16齿长矛齿轮设置为有效组件，然后单击草图
<br>
<img src="PM/CAD/Plugin/figure19.png" style="float: center;" width=700 > 
<br>

单击此齿轮的脸并选择捕获位置
<img src="PM/CAD/Plugin/figure20.png" style="float: center;" width=700 > 
<br>
然后按P进行项目。然后在当前草图上选择输入轴直径作为几何。单击确定，然后单击完成草图
<img src="PM/CAD/Plugin/figure21.png" style="float: center;" width=700 > 
<br>
按E排除E，然后选择该输入轴直径作为配置文件，将距离设置为-40mm，在操作选项上选择一个连接以加入轴
<img src="PM/CAD/Plugin/figure22.png" style="float: center;" width=700 > 
<br>
让我们将矛齿轮（32齿）重命名为行星齿轮和刺齿轮（16齿），因为太阳齿轮只是要组织起来
<img src="PM/CAD/Plugin/figure23.png" style="float: center;" width=700 > 
<br>
现在看一下草图的前 /顶 /后部 /底部视图，齿轮不是集体游行。
<img src="PM/CAD/Plugin/figure24.png" style="float: center;" width=700 > 
<br>
现在按M并选择旋转，然后选择要移动的组件，而轴是齿轮的中心，然后手动旋转齿轮的位置，直到它们正确匹配为止。对于其余的齿轮，请执行同样的操作，直到它们完全匹配为止。
<img src="PM/CAD/Plugin/figure25.png" style="float: center;" width=700 > 
<br>
一旦一切都正确匹配，请捕获位置
<img src="PM/CAD/Plugin/figure26.png" style="float: center;" width=700 > 
<br>

现在，最后一部分是将每个行星齿轮连接到输入轴的载体。通过选择创建然后选择新组件来创建新组件
<img src="PM/CAD/Plugin/figure27.png" style="float: center;" width=700 > 
<br>
命名组件“载体”，然后单击“好” 
<img src="PM/CAD/Plugin/figure28.png" style="float: center;" width=700 > 
<br>
通过单击草图创建一个新草图，然后将鼠标放在一个平面齿轮之一的脸上
<img src="PM/CAD/Plugin/figure29.png" style="float: center;" width=700 > 
<br>
单击P进行投影并选择齿轮的所有内径，如下所示，请单击“确定”
<img src="PM/CAD/Plugin/figure30.png" style="float: center;" width=700 > 
<br>
选择中心直径圆，并在所有齿轮中创建直径为10直径的圆。确保缩小齿轮的中心以将鼠标放置以进行绘制。
<img src="PM/CAD/Plugin/figure31.png" style="float: center;" width=700 > 
<br>
选择Aline加入所有齿轮。绘制连接所有齿轮的载体线
<img src="PM/CAD/Plugin/figure32.png" style="float: center;" width=700 > 
<br>
选择标记以确保线将线连接到圆上。选择几何图形，这是线条，每个点处的齿轮圆与线接触EG，如下所示
<img src="PM/CAD/Plugin/figure34.png" style="float: center;" width=700 > 
<br>
选择在交叉路口上指定半径的圆角。选择两行进行交集，然后单击确定并完成草图
<img src="PM/CAD/Plugin/figure33.png" style="float: center;" width=700 > 
<br>

按E在键盘上排除。在配置文件上，选择齿轮的所有直径和轴的所有侧面（6个组件），如下所示，并设置其他参数，如图所示
<img src="PM/CAD/Plugin/figure35.png" style="float: center;" width=700 > 
<br>
掩盖身体组件并揭示载体的草图组件，如下所示。按E再次排除。在配置文件上仅选择Plannet齿轮的直径和（3个内圆的Atotal），并设置其他参数，如图所示
<img src="PM/CAD/Plugin/figure36.png" style="float: center;" width=700 > 
<br>
揭开载体的身体组件，然后按E再次排除E。在配置文件上，仅选择Plannet齿轮的直径，（3个内圆的Atotal）设置参数如下所示，然后单击“确定”
<img src="PM/CAD/Plugin/figure37.png" style="float: center;" width=700 > 
<br>
揭开运营商的草图组件，然后单击草图，然后选择ATH载体作为平面
<img src="fPM/CAD/Plugin/igure38.png" style="float: center;" width=700 > 
<br>

单击P进行项目，然后选择Sun Gear SA几何形状选项的中心
<img src="PM/CAD/Plugin/figure39.png" style="float: center;" width=700 > 
<br>
在太阳齿轮的中心创建直径为5mm的圆圈，然后单击“确定”并完成草图。
<img src="PM/CAD/Plugin/figure40.png" style="float: center;" width=700 > 
<br>

按E再次排除。在配置文件上，仅选择上面创建的太阳齿轮的直径，并设置其他参数，如图所示。此移动连接所有齿轮。注意：有时候，选择此内圆可能很难掩盖其他图层，例如身体，素描以选择此圆圈并在选择它之后将其放置。
<img src="PM/CAD/Plugin/figure41.png" style="float: center;" width=700 > 
<br>
现在，已经创建了载体连接到齿轮，现在模式已完成。
现在让我们定义关节。我们将用作构建关节，但首先让我们定义载体和每个平面图之间的关节。
选择组装并作为建筑联合选项
<img src="PM/CAD/Plugin/figure47.png" style="float: center;" width=700 > 
<br>
<br>
将参数设置为如下运动类型Revolute，首先选择“平面齿轮”，然后选择载体作为组件，然后选择“行星齿轮中心”作为快照（请记住要缩放中心）。
<img src="PM/CAD/Plugin/figure48.png" style="float: center;" width=700 > 
<br>
<br>
在其余的行星齿轮中重复此过程。注意：有时，很难选择平面齿轮和载体，尝试掩盖载体以选择行星齿轮组件并卸载载体并选择载体组件。
一开始，定义环齿轮已固定，现在让我们去戒指并选择地面以将其固定在适当的位置
<img src="PM/CAD/Plugin/figure49.png" style="float: center;" width=700 > 
<br>
<br>
现在，让我们定义托架和环齿轮，太阳和环齿轮之间的接头。
选择组装并选择作为建造接头，然后选择载体和环齿轮作为组件和中心为载齿轮的中心。对带环齿轮的载体和太阳齿轮重新修复，然后将连接命名为
<img src="PM/CAD/Plugin/figure50.png" style="float: center;" width=700 > 
<br>
<br>

让我们应用每个齿轮组件之间的运动链接。选择组装并选择运动链接
<img src="PM/CAD/Plugin/figure51.png" style="float: center;" width=700 > 
<br>
<br>
从关节菜单中创建一个在太阳环和载波环之间的运动链接，并设置其他参数，如下所示
<img src="PM/CAD/Plugin/figure52.png" style="float: center;" width=700 > 
<br>
<br>
在太阳齿轮和每个平面图之间建立一个运动链接。选择和选择运动链接。选择太阳环和平面载体。重复两个平面齿轮中其余的过程
<img src="PM/CAD/Plugin/figure53.png" style="float: center;" width=700 > 
<br>
<br>
当我们尝试旋转太阳齿轮时，现在看起来不好
<img src="PM/CAD/Plugin/figure54.png" style="float: center;" width=700 > 
<br>
<br>
重命名要组织的运动链接
<img src="PM/CAD/Plugin/figure55.png" style="float: center;" width=700 > 
<br>
<br>
现在编辑太阳和行星之间的运动链接
<img src="PM/CAD/Plugin/figure56.png" style="float: center;" width=700 > 
<br>
<br>
在太阳（首先选择）和平面链接之间设置关节的pameter，并在最后两个关节的齿轮齿轮的最后两个接头中重复使用，如下所示。现在，如果您旋转太阳装备，一切都正确匹配
<img src="PM/CAD/Plugin/figure57.png" style="float: center;" width=700 > 
<br>
<br>
该模型已经完成并且正在采取行动
<img src="PM/CAD/Plugin/figure59.png" style="float: center;" width=700 > 
<br>
<br>