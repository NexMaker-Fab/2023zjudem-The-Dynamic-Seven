# 在这里，我们将成为Cardan关节

**工具和命令**

- 成分
- 关节
- 洞
- 挤出（旋转）
- 结合
- 挤出（切割）
- 圆角



在这里，我们可以看到以厘米为单位的所有维度。我们的基本结构。
<BR>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/1.png">
<BR>
选择新设计。我们可以从文件选项或快捷方式“ CTRL+N”打开它。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/2.png">
<BR>
“ Ctrl+S”这里我们可以添加我们的模型名称并保存它。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/3.png">
<BR>
对于此模型，我们将使用以厘米为单位的所有单元。从这里我们将单元更改为厘米。<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/4.png">
<BR>
从组装选项中，我们创建了新组件。<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/5.png">
<BR>
选择新组件，然后从创建选项创建一个新草图，然后选择一个平面。在这里我们选择正面部分。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/6.png">
<BR>
选择矩形这次我们使用了中心矩形。使矩形4,6。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/7.png">
<BR>
从修改中，选择偏移量选项make -1.cm偏移量。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/8.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/9.png">
<br>
单击完成草图
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/10.png">
<BR>

**拉伸**
创建草图后，从工具栏或右键单击上下文菜单中选择“挤出”命令。您还可以在“创建”下拉菜单中找到它。在要挤出的草图区域上单击。选定的区域将突出显示。

Fusion 360现在将显示“挤出”对话框。在这里，您可以设置几个参数：

 - 距离：指定要在第三维中划出草图的距离。您可以输入特定值或在图形区域拖动箭头。

 - 方向：选择是在一个方向上挤出，对称两侧还是在特定的面或平面上。

 - 操作：您可以执行各种操作，例如“ JOIN”，“ CUT”，“ Intersect”或“ New Body”。这决定了挤出与现有几何形状相互作用的方式。

 - 锥度角度：如果需要，可以通过指定角度添加锥度。

 - 开始：结束：使用这些选项来指定挤压相对于草图的何时启动和结束。如果您选择“新主体”操作，则可以使用这些参数。
 - 单击“挤压”对话框中的“确定”按钮以确认并创建3D对象。
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/11extrude.png">
<BR>
使新草图在对象的中心中旋转两个圆圈。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/11.1.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/12.png">
<BR>
完成草图
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/13.png">
<BR>
选择小圆圈，操作“切割”距离-3.50cm。它将切割对象。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/14.png">
<BR>
现在选择这次加入操作的大圆圈。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/16.png">
<BR>

**圆柱**

 - 选择要在其上创建气缸的平面。
 - 要创建一个圆柱体，请转到“创建”下拉菜单，然后从“原始人”部分中选择“气缸”。
 - 单击您想要圆柱底座中心的草图平面中的位置。
 - 拖动光标或输入值以定义圆柱体底部的直径。
 - 现在，您需要指定气缸的高度。您可以将光标拖到所需方向或输入特定值。
 - 指定基本中心，直径和高度后，单击以确认气缸创建。
 - 一旦您对气缸感到满意，请单击“ OK”或“ Enter”来完成该功能，以退出草图环境并完成气缸。

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/17cylinder.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/18cylinder.png">
<BR>

**鱼片**

 - 选择对象或要填充的边缘后，转到“修改”下拉菜单，然后选择“ Fillet”命令。
 - 单击您要舍入的边缘或面孔。Fusion 360将突出所选区域。
 - 在“圆角”对话框中，您需要指定圆角半径。这决定了圆形区域的大小。您可以输入特定值，也可以使用滑块进行交互调整半径。
-Additional选项（可选）：
Fusion 360在“ Fillet”对话框中提供其他选项，包括：

脸部圆角：如果您选择的面孔，则可以选择创建一个圆形的圆角。
多个圆角：您可以选择多个边缘或面孔以在一个操作中填充。
对称圆角：在边缘上创建一个对称圆角。
切线链：自动选择连接的边缘或面链以圆角。

调整圆角参数时，Fusion 360将提供圆角边缘或面的实时预览。确保结果看起来像您想要的方式，然后单击确定。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/19fillet.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/20fillet.png">
<BR>

**镜子**

 - 选择要镜像的组件或功能。这可以是草图，车身，组件或孔，挤出或圆角等功能。
 - 有几种访问镜像命令的方法：

   - 转到“模式”部分的“创建”下拉菜单，然后选择“镜像”。
   - 右键单击要在Fusion 360图形区域或Fusion 360浏览器中镜像的对象上，然后从上下文菜单中选择“镜像”。
 - 有几种访问镜像命令的方法：

 - 转到“模式”部分的“创建”下拉菜单，然后选择“镜像”。
 - 右键单击要在Fusion 360图形区域或Fusion 360浏览器中镜像的对象上，然后从上下文菜单中选择“镜像”。

 - 在“镜像”对话框中，选择要在镜像操作中包含的组件。您可以选择原始对象，镜像或两者兼而有之。确保根据您的设计需求选择适当的选项。
 -  Fusion 360将提供镜像对象及其位置的实时预览。确保结果与您的设计意图保持一致。
 - 对预览感到满意后，单击“镜像”对话框中的“确定”按钮以确认并应用镜像操作。
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/21m.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/22m.png">
<BR>

**复制**

 - 选择要复制的组件，功能，草图或对象。
 - 有几种访问复制命令的方法：

   - 转到“修改”下拉菜单，然后从“移动/复制”部分中选择“复制”。
   - 右键单击Fusion 360图形区域或Fusion 360浏览器中的选定对象，然后从上下文菜单中选择“复制”。
 -  Fusion 360将提示您指定参考点。单击对象的特定点或边缘，该点将用作重复的参考。
 - 单击要放置对象副本的位置。您可以将对象拖动到所需的位置，也可以输入特定的坐标。
 - 指定复制点，目标点和任何其他设置后，单击“复制”对话框中的“确定”按钮以确认并创建复制。
 - 在这里，您可以看到我们的第二个组件是组件的副本。
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/23copy.png">
<BR>
从组装选择新组件。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/24new_com.png">
<BR>
做另一个圆柱体。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/25make_cylinder.png">
<BR>

**结合**

 - 首先选择要组合的3D主体，组件或功能。这些可以是设计中的身体，组件或功能。您可以在图形区域或Fusion 360浏览器中直接选择它们。
 - 以以下方式之一访问联合命令：
   - 转到“修改”下拉菜单，然后从“联合收割机”部分中选择“组合”。
   - 右键单击Fusion 360图形区域或Fusion 360浏览器中的选定对象之一，然后从上下文菜单中选择“组合”。

<B>合并操作</B>

在“组合”对话框中，您将拥有以下组合操作的选项：

 - 加入：这将所选对象组合到一个合并的身体中。

*剪切：这将所选对象彼此减去，在它们相交的地方创建一个切割或空隙。
 - 相交：这仅保留所选对象的公共区域，丢弃其余的对象。

 - “切割”操作，您需要指定目标和工具主体。目标主体是您要切割的对象，而工具主体是用于执行切割的对象。Fusion360将提供联合操作结果的实时预览。确保预览与您的设计意图匹配，然后单击“确定”。

<br>
<img style="float: center;" width=1000 src="PM/CAd/cad_img/26combine.png">
<BR>

使用圆角选项。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/27.png">
<BR>

使用移动功能制作引脚1的副本。并制作引脚2。

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/28.png">
<BR>

**新组件**

 - 首先打开现有设计或在Fusion 360中创建新设计。
 - 有几种创建新组件的方法：
   - 在Fusion 360浏览器中，右键单击顶级组件（通常命名为“ Component1”）或现有组件，然后选择“新组件”。
   - 转到“汇编”下拉菜单，然后选择“新组件”。
创建空组件：此选项创建一个没有几何形状的空组件。然后，您可以根据需要向其添加草图，身体和功能。
指定组件名称并选择创建方法后，单击“确定”按钮以创建新组件。

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/29cb.png">
<BR>

**项目**

“项目”功能是在3D表面上创建参考几何形状或捕获2D草图的有用工具。它允许您将特定的几何形状或信息从3D模型传输到2D草图。这是项目功能的工作方式：

有几种访问项目命令的方法：

 - 在草图工作区中，转到“创建”下拉菜单，然后选择“ insert”部分中的“项目/include”。
 - 在草图环境中，右键单击“草图”调色板或现有的草图实体，然后从上下文菜单中选择“ project/include”。
 - 您可以在键盘上单击“ P”项目命令将运行。

单击要投影到当前草图中的3D模型的边缘，面或其他几何形状。Fusion 360将突出显示所选的几何形状。

选择几何形状后，您可能需要指定投影发生的方向。Fusion 360将默认情况下垂直于草图平面投射所选的几何形状。但是，如果需要，您也可以设置自定义投影方向。

Fusion 360将将选定的3D几何形状投射到您的草图平面上。您会看到投影线和点的实时预览。确保投影与您的设计意图保持一致。

对投影感到满意后，单击“项目”对话框中的“确定”按钮以确认并创建草图实体。
将PIN1上部作为项目。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/30project.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/31project.png">
<BR>
  
**草图维度**

将尺寸添加到融合360中的草图是创建精确和参数2D几何形状的重要步骤。这是将尺寸添加到草图的方法：

 - 首先要么在特定平面上创建新草图，要么在Fusion 360中打开现有草图。
 - 在草图工作区中，选择“草图维度”工具。您可以在“草图”下拉菜单或工具栏中找到它。
 - 单击您要尺寸的草图实体（线，弧，圆形等）。Fusion 360将突出显示所选实体。
 - 单击要放置维度的位置。此操作将创建一个维线，并且将出现维数值。您可以将尺寸值拖动以在需要时重新定位。
 - 放置尺寸后，您可以在键盘上键入特定值，也可以拖动尺寸线以设置所需的尺寸。Fusion 360将自动更新草图几何形状以匹配新维度。
 - 在Fusion 360浏览器中，您会发现“素描调色板”。它提供了尺寸，约束和草图实体的列表。您可以使用草图调色板轻松管理和编辑草图的尺寸和约束。

这里首先选择中心块。
创建新草图。
选择圆。
使两个圆的小对方具有1厘米的尺寸，而另一个2厘米尺寸。
选择草图维度。
首先，选择项目线，然后选择圆心中心，然后在2厘米和1厘米之间进行垂直距离。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/32.png">
<BR>
完成草图后。
现在使用挤出命令。
选择中心块，然后选择挤出。
现在，选择此处的配置文件选择1厘米圆和方向对称。距离1.25 cm操作新身体。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/33cb.png">
<BR>
现在选择挤出命令
同时选择1cm和2cm圆圈。
从对象开始操作。
距离1厘米
选择“加入”操作
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/34cb.png">
<BR>
在中心块中选择镜子。
在镜子中选择对象类型“功能”
选择在中心块中挤出的对象
选择镜平面作为图像
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/35cb.png">
<BR>
现在复制并移动。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/36cb.png">
<BR>

制作一个新的草图。打开项目，然后选择左圆作为图像。现在，用5厘米和1厘米制作矩形。
选择草图尺寸，并在圆形中心和矩形5厘米线之间建立0.5 cm的距离。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/37cb.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/38cb.png">
<BR>

现在挤出选定的部分。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/39cb.png">
<BR>
使用Mirror命令。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/40.png">
<BR>
这是我们的所有组件。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/41all_com.png">
<BR>
现在，我们添加一些将成为我们的基础的其他组件。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/42.png">
<BR>
制作并移动它。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/43.png">
<BR>
使组件4.1接地。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/44ground.png">
<BR>

**联合的**

在Fusion 360中进行联合设计的工作涉及建立3D模型中组件或身体之间的连接和关系，以模拟它们如何相互移动和相互作用。关节对于设计组件是必不可少的，尤其是如果您想测试零件如何结合在一起以及它们在制造前的移动方式。这是如何在Fusion 360中与关节合作的基本概述：

确保您的设计中有多个组件或物体，要使用关节连接。如果不这样做，则可能需要创建其他组件。

激活关节工具：

单击工具栏中的“组装”工作区以访问汇编工具。
从“组装”菜单中选择“联合”命令。

选择组件：使用“选择”工具选择要加入的组件或物体。通常，您选择两个组件来定义关节。

选择关节类型：Fusion 360提供各种类型的关节来模拟不同类型的运动。一些常见的联合类型包括：

Revolute关节：模拟旋转运动，例如铰链或枢轴。
滑块接头：像滑动抽屉一样模拟线性运动。
圆柱接头：结合了翻译和旋转运动。
平面关节：限制组件在飞机上移动，例如滑门。
球接头：允许在多个轴上进行旋转运动，例如球和插座接头。

配置关节参数：根据您选择的关节类型，Fusion 360会要求您定义参数。这可能包括指定旋转接头的旋转轴，滑块接头的线性运动方向或其他相关参数。

测试组件：创建关节后，您可以使用“运动研究”功能来测试组件如何移动和相互作用。这可以帮助您确保您的设计按预期工作。

在这里首先选择一个组件和地面。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/45j.png">
<BR>

在这里，我们可以在关节之后看到。

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/46.png">
<BR>

现在加入引脚和洋子。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/47.png">
<BR>

检查运动。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/48j.png">
<BR>

现在加入PIN和中心块
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/49j.png">
<BR>

调整销钉和中心块位置。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/50j.png">
<BR>
选择另一个PIN和中心块并加入它们。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/51.png">
<BR>
调整位置。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/52.png">
<BR>
现在，另一个选择洋子和销钉。并加入它们。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/53.png">
<BR>
加入洋子
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/54.png">
<BR>
现在，我们可以看到所有组件加入。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/55all.png">
<BR>
现在设置移动旋转。单击键盘上的M，首先选择Yoko 1，然后选择PIN。在再次选择销钉后，请再次选择Yoko。现在以22.5度以Z角度调整引脚。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/56.png">
<BR>

调整了该学位后，我们的最终3D模型。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/57final.png">
<BR>
为了更好地查看隐藏组件4.1和组件4.2。
在此处转到接头文件，然后单击Revolute 6中鼠标中的右键。然后选择Animate关节关系。
现在我们可以看到我们的最终模型。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/58.png">
<BR>

**外貌**

使用Fusion 360中的“外观”功能，您可以将各种视觉属性应用于3D型号，以使它们看起来更加现实。这些外观可以模拟现实世界中材料和饰面的方式。这是Fusion 360中使用外观的方法：

在工具栏中，单击“外观”图标，该图标看起来像油漆桶。

在外观面板中，您可以浏览预定义外观的库。您可以从木材，金属，塑料，玻璃等材料中进行选择。有多种选择。

要将外观应用于模型的一部分，请通过在工作区中单击它或从模型树中选择它来选择零件。
选择零件后，通过单击外观面板选择所需的外观。

应用外观后，您可以进一步自定义。单击外观面板中的外观，您将看到调整属性等属性等选项，例如颜色，光泽，凹凸和透明度。

您可以通过调整透明度滑块来使材料透明。

如果您创建了将来要重复使用的自定义外观，则可以将其保存为自定义外观。
将外观应用到不同部分：

您可以在模型的不同部分应用不同的外观，以模拟不同的材料和饰面。
渲染您的模型：

要在其完整的荣耀中查看外观，您可以使用Fusion 360的渲染功能。这将为您提供模型的影像逼真的表示，并具有应用外观。
保存和导出：

对外观满意后，保存模型并以所需格式导出以进行演示或制造。
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/59.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/60color.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/cad.gif">
<BR>

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6eed5131418f6a02c7?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


## 如何将项目添加到我们的网站 [Myhub Autodesk360](https://myhub.autodesk360.com/)

1. 在我们的机器中打开Fusion 360，然后选择我们的项目。首先检查离线或在线检查。如果离线选择在线选择。
<br>

<img style="float: center;" width=1000 src="PM/CAD/add_1.png">
<BR>
2. 单击数据面板，然后单击网络上的打开。
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_2.png">
<BR>
3. 单击您的项目。
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_3.png">
<BR>
4. 单击共享链接并打开它。
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_4.png">
<BR>
5. 选择嵌入并复制链接。
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_5.png">
<BR>

6. 经过网站上的链接。

         **MINHAZULISLAM**
         <iframe src="https://a360.co/3MbfPle" width="640" height="480" allowfullscreen="true"          webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
         <BR>
         <br>
         <img style="float: center;" width=1000 src="PM/CAD/cad.gif">
         <BR>
         **TASNIM AFRA**
         <iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e262a460a6399672d?         mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true"          mozallowfullscreen="true"  frameborder="0"></iframe>
         <BR>
         <img style="float: center;" width=1000 src="PM/CAD/afra.gif">
         <BR>

7. 我们添加了此代码的GIF

         <BR>
         <img style="float: center;" width=1000 src="PM/CAD/afra.gif">
         <BR>
