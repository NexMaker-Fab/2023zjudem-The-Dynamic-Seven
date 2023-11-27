# **Pluging**

In Fusion 360, a plugin (sometimes referred to as an "add-in") is a piece of software that extends the functionality of the core Fusion 360 application. These plugins are typically created by third-party developers or users and can be installed to provide additional features, tools, or capabilities within Fusion 360. Plugins can be used to streamline specific workflows, add new design or simulation tools, integrate with external software or hardware, and much more.

Here are some common uses for Fusion 360 plugins:

1. Custom Tools: Plugins can add custom design, simulation, or manufacturing tools tailored to specific needs that may not be available in the core software.

2. File Import/Export: Plugins can support various file formats for importing or exporting designs, allowing for interoperability with other software.

3. Automation: Plugins can automate repetitive tasks or create custom scripts to perform design operations efficiently.

4. Data Management: Some plugins assist in data management, helping users organize and track design data more effectively.

5. Integration: Plugins can integrate Fusion 360 with external applications or hardware, enhancing its capabilities for specific industries or processes.

6. Simulation and Analysis: Certain plugins offer advanced simulation and analysis capabilities, such as finite element analysis (FEA) or computational fluid dynamics (CFD).

7. CAM (Computer-Aided Manufacturing): CAM plugins can help generate toolpaths for CNC machining and other manufacturing processes directly from Fusion 360.

8. Rendering and Visualization: Plugins can improve rendering and visualization capabilities, enabling more realistic 3D renderings of designs.
   

   <br>
   <br>

## Planetary Gear Train Modeling
<br>
<br>


A planetary gear train is a mechanical system consisting of gears arranged in a specific configuration known as a planetary or epicyclic gear arrangement. It comprises three main components: a sun gear positioned at the center, planet gears that revolve around the sun gear, and a ring gear enclosing the planet gears. These gears are interconnected in a way that enables them to transmit motion and torque in complex but predictable ways.

Modeling a planetary gear train involves understanding and mathematically representing its behavior. Engineers and mathematicians use equations and diagrams to describe how the gears interact, the speed ratios, torque transmission, and rotational direction changes within the system.

To model a planetary gear train, one typically considers factors like the number of teeth on each gear, gear sizes, rotational speeds, and the gear arrangement. Equations derived from the principles of gear mechanics, such as the laws of gearing and kinematics, are used to predict and analyze the system's performance. Computer simulations and mathematical models help in understanding the behavior of the gear train under different conditions and configurations.

Modeling planetary gear trains is crucial in various fields, including mechanical engineering, automotive design, robotics, and more, as it allows engineers to predict performance, optimize designs, and ensure efficient power transmission within machinery and systems.
<br>
<br>

**3D Model**

Setting up design parameters
This project will build a gear with contain three gear namely ring, sun and  planent. The gear ration 1:6, fixed:Ring Gear,driven: Sun Gear, Output: Carrier 

Open the fusion 360 application.

Select the utility in the fusion task bar.

<br>
<img src="PM/CAD/Plugin/figure1.png" > <br>
<br>
Select ADD-INS and Select Scripts and Add-Ins option ( or click Shift + S). This pops scripts and Add-Ins box options on the screen.
<br>
<img src="PM/CAD/Plugin/figure2.png" > <br>
<br>

Click Add-Ins option, scrowl down and Select the SpearGear option and click run.This add a SpearGear command in the <b>Create</b> pannel. Click OK on the command sample popup. 
<br>
<img src="PM/CAD/Plugin/figure3.png" style="float: center;" width=700 > <br>
<br> <br>
Click Solid on the fusion workplace and  click Create option and Select the SpearGear on the create options.
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
<br>

Set up the Spur Gear parameter as shown below and click OK. This create a SpurGear with 80 teeth but we want an inverse.
<br>
<img src="PM/CAD/Plugin/figure5.png" style="float: center;" width=700 > <br>
<br>

Click Create and select Cylider.Select any plane and sketch the cylider from the center of the circle.
<br>
<img src="PM/CAD/Plugin/figure6.png" style="float: center;" width=700 > <br>
<br>
Set up the parameters as shown below and click OK
<br>
<img src="PM/CAD/Plugin/figure7.png" style="float: center;" width=700 > <br>
<br>
Now we gonna use the extrude command to cut the shape of the gear from the cyclider. Activate the cyclider  
<br>
<img src="PM/CAD/Plugin/figure8.png" style="float: center;" width=700 > <br>
<br>
Press E for extrude. Set the  distance to -10mm and select the spear gear as a profile and other parameters as shown below.Note :profile options; click the face of the gear to select it
<br>
<img src="PM/CAD/Plugin/figure9.png" style="float: center;" width=700 > <br>
<br>
Now select the SpearGear(80teeth)  component  and Right click the spearGear(80teeth). Select  Remove option and Click Ok
<br>
<img src="PM/CAD/Plugin/figure10.png" style="float: center;" width=700 > <br>
Double click the componenent 2 and rename it to the Ring gear
<br>
<img src="PM/CAD/Plugin/figure11.png" style="float: center;" width=700 > <br>
Now lets modal the planents.Create another supergear by Clicking the CREATE and select the spear gear option.
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
Set up the parameters as shown below. The rest of the parameters will remain the same except for the number of teeth will be 32 and other two parameters as shown below and click OK
<br>
<img src="PM/CAD/Plugin/figure12.png" style="float: center;" width=700 > <br>
Press M on the keyboard to move the component  and Select Components on move object option in the Move/Copy menu and zoom in the origin to select the origin to be center as select option. Check the create Copy option first and set the y axis to 48mm  The aim is to make a copy of the gear.
<br>
<img src="PM/CAD/Plugin/figure13.png" style="float: center;" width=700 > <br>

Press M again and  this time add rotation as motion type, select the axis to be center of the gear and set the angle to 120 degrees.Check the create Copy option first. The aim is to make another copy of the gear
<br>
<img src="PM/CAD/Plugin/figure14.png" style="float: center;" width=700 > <br>

Before clicking OK,  Check free mode and set the y axis to 48mm  and click OK
<br>
<img src="PM/CAD/Plugin/figure15.png" style="float: center;" width=700 > <br>
Press M again and  add rotation as motion type, select the axis to be center of the gear and set the angle to 240 degrees. Do not check the copy option because this is a last copy
<br>
<img src="PM/CAD/Plugin/figure16.png" style="float: center;" width=700 > <br>

Before Clicking Ok, Check free mode and set the y axis to 48mm  and click OK. 
<br>
<img src="PM/CAD/Plugin/figure17.png" style="float: center;" width=700 > <br>
The planet gear are now in place.Now lets modal the sun gear with 16 teeth.
Create another supergear by Clicking the CREATE and select the spear gear option 
<br>
<img src="PM/CAD/Plugin/figure4.png" style="float: center;" width=700 > <br>
Set up the parameters as shown below. The rest of the parameters will remain the same except for the number of teeth  which will be 16 and click OK
<br>
<img src="PM/CAD/Plugin/figure18.png" style="float: center;" width=700 > <br>
The sun gear is now in place.Lets now build an input shaft to the 16 teeth spear gear.
Set the 16 teeth  spear gear as an  active components and click the sketch
<br>
<img src="PM/CAD/Plugin/figure19.png" style="float: center;" width=700 >

Click the face of this gear and Select the capture position 
<img src="PM/CAD/Plugin/figure20.png" style="float: center;" width=700 > <br>
Then press P to project. Then select the input shaft diameter as geometery on the current sketch. Click OK and click finish sketch
<img src="PM/CAD/Plugin/figure21.png" style="float: center;" width=700 > <br>
Press E for exclude and select that input shaft diameter as a profile, set distance to -40mm, select a join on operation options to join to the shaft
<img src="PM/CAD/Plugin/figure22.png" style="float: center;" width=700 > <br>
Let's rename the spear Gear (32teeth) as a planent gear and spear gear (16teeth) as the Sun gear just to be organised 
<img src="PM/CAD/Plugin/figure23.png" style="float: center;" width=700 > <br>
Now take alook at the front/top or back /bottom view of the sketch ,the gears are not marching collectively.
<img src="PM/CAD/Plugin/figure24.png" style="float: center;" width=700 > <br>
Now press M and select rotate then pick the components you want to move and the axis which is the center of the gear then manually rotate the position of the gear until they match correctly. Do the same for the rest of the gears until they are fully matched.
<img src="PM/CAD/Plugin/figure25.png" style="float: center;" width=700 > <br>
Once everything is matching correct , capture the position
<img src="PM/CAD/Plugin/figure26.png" style="float: center;" width=700 > <br>

Now the last part is the carrier which is the one which is going to connect each of the planet  gears to the input shaft.
Create anew component by selecting CREATE then select new component 
<img src="PM/CAD/Plugin/figure27.png" style="float: center;" width=700 > <br>
Name the component "Carrier" and click okay 
<img src="PM/CAD/Plugin/figure28.png" style="float: center;" width=700 > <br>
create a new sketch by click sketch and position the mouse on the face of one of the  planent gear 
<img src="PM/CAD/Plugin/figure29.png" style="float: center;" width=700 > <br>
click P to project and select all the  inner diameter of the gears as shown below and click OK
<img src="PM/CAD/Plugin/figure30.png" style="float: center;" width=700 > <br>
select Center Diameter Circle and create circles of 10 diameter in all the gears. make sure to zoom the center of the gear to position the mouse for drawing.
<img src="PM/CAD/Plugin/figure31.png" style="float: center;" width=700 > <br>
Select aline to join all the gears.Draw the carrier lines that connect all the gears as shown below
<img src="PM/CAD/Plugin/figure32.png" style="float: center;" width=700 > <br>
Select the tagent to make sure that the lines are attached to the circle.Select the geometery which is the line and the gear circle at each point the circle become in contact with the line eg as shown below
<img src="PM/CAD/Plugin/figure34.png" style="float: center;" width=700 > <br>
select fillets to specify the radius at the intersection.Select the two separate lines making the intersection and click OK and finish sketch 
<img src="PM/CAD/Plugin/figure33.png" style="float: center;" width=700 > <br>

Press E for exclude on keyboard. On profile select all the diameters of the gears and all the sides of the shaft(6components) as shown below and set the other parameters as shown
<img src="PM/CAD/Plugin/figure35.png" style="float: center;" width=700 > <br>
mask the body component  and unmask the sketch  component of the carrier  as shown below. Press E for exclude again. On profile only select  the diameters of the plannet gears and (atotal of 3 inner circle) and set the other parameters as shown
<img src="PM/CAD/Plugin/figure36.png" style="float: center;" width=700 > <br>
Unmask the body component  of the carrier and
Press E for exclude again. On profile only select  the diameters of the plannet gears and (atotal of 3 inner circle)   set the parameters as shown as shown below and click OK
<img src="PM/CAD/Plugin/figure37.png" style="float: center;" width=700 > <br>
UnMask the sketch component  of the carrier  and click sketch and select athe carrier as the plane  
<img src="PM/CAD/Plugin/figure38.png" style="float: center;" width=700 > <br>

Click P for project and  select the center of the sun gear sa geometry option
<img src="PM/CAD/Plugin/figure39.png" style="float: center;" width=700 > <br>
Create a circle of diameter of 5mm at the center of sun gear and click Ok and finish sketch .
<img src="PM/CAD/Plugin/figure40.png" style="float: center;" width=700 > <br>

Press E for exclude again. On profile only select  the diameters of the sun gears created above and set the other parameters as shown. This shift connect all the gears.Note: sometimes, it might be difficult to select this inner circle, try to mask other layers like body, sketch  to  select this circle and umask them after selecting it.
<img src="PM/CAD/Plugin/figure41.png" style="float: center;" width=700 > <br>

Now the carrier has been created connected to the gears and now the modal is complete. 
Now lets define the joints. we will use AS Build Joint but first lets define the joints between the carrier and each planent .
Select Assemble and as build joint option
<img src="PM/CAD/Plugin/figure47.png" style="float: center;" width=700 > <br>
<br>
set the parameters as follows motion type revolute,select planent gear first and carrier as  components then select the center of planet gear as snap(remember to zoom the center).
<img src="PM/CAD/Plugin/figure48.png" style="float: center;" width=700 > <br>
<br>
Repeat this process for the rest of the planet gear. Note: sometimes, it might be difficult to select the planent gear and carrier, try to mask the carrier to select the planet gear component and umask the carrier and select the carrier component.
At the beginning, the ring gear is defined being fixed, now lets go to ring gear and choose ground to hold it in place
<img src="PM/CAD/Plugin/figure49.png" style="float: center;" width=700 > <br>
<br>
Now lets define the joint between the carrier and ring gear , the sun and ring gear.  
Select assemble and select As build joint and select the carrier and ring gear as component and center be the center of carrier gear.Repeat this for the carrier and sun gear with ring gear and rename the join as shown below
<img src="PM/CAD/Plugin/figure50.png" style="float: center;" width=700 > <br>
<br>

let's apply the motion links between each gear components. Select Assemble and select motion links
<img src="PM/CAD/Plugin/figure51.png" style="float: center;" width=700 > <br>
<br>
create a motion link between the sun ring and the carrier  ring from the joint menu and set up other parameters as shown below
<img src="PM/CAD/Plugin/figure52.png" style="float: center;" width=700 > <br>
<br>
create a motion link between gear between the sun gear and each of the planents.Select Assemble and select motion links. select the sun ring and the planent carrier. Repeat the process for the rest of the two planent gears
<img src="PM/CAD/Plugin/figure53.png" style="float: center;" width=700 > <br>
<br>
As we try to rotate the sun gear, it does not look good now edit the motion links between the sun ring and the carrier joint and set the parameters below
<img src="PM/CAD/Plugin/figure54.png" style="float: center;" width=700 > <br>
<br>
Rename the motion links to be organised
<img src="PM/CAD/Plugin/figure55.png" style="float: center;" width=700 > <br>
<br>
Now edit the motion link between the sun and planets
<img src="PM/CAD/Plugin/figure56.png" style="float: center;" width=700 > <br>
<br>
set the pameters of the joint between the sun(first to select) and planent links and repeat the same for the last two joints of planet gear as  shown below. Now if you rotate the sun gear, everything matches correctively
<img src="PM/CAD/Plugin/figure57.png" style="float: center;" width=700 > <br>
<br>
The model is complete and in action
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

Here we create a Create Spur gears. In this part we using plugins to create spur gears.

<img style="float: center;" width=1000 src="PM/CAD/fg/1st.jpg">

<br> 
At first go to the Fusion 360 main Interface then this page arrived. 
<br><br>
<br> 

<img style="float: center;" width=700 src="PM/CAD/fg/2nd.jpg">
<br><br>
Then Select Utilities.
<br>
<br>

<img style="float: center;" width=700 src="PM/CAD/fg/3rd.jpg">
<br<br>>

Then go to "ADD-IN" Option then select "Fusion 360 APP Store ".  

<br><br>
<img style="float: center;" width=700 src="PM/CAD/fg/4th.jpg">
<img style="float: center;" width=700 src="PM/CAD/fg/5th.jpg">
<br> <br>
Then just go and search for "FM Gear" after that download it . After installation FM Gear Pluging option is appeared in the Solid-Create-FM Gear. 
<br><br>
<img style="float: center;" width=700 src="PM/CAD/fg/6th.jpg">
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/7th.jpg">
<br>
Now we can see that this FM Gear is arraived. After Clicking there this page arrived. After fix everything press ok then one gear arrived. 

<br>
<br>
<img style="float: center;" width=700 src="PM/CAD/fg/8th.jpg">

<br>
This is our one gear. Now we also add one gear. 
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/9th.jpg">
 
<img style="float: center;" width=700 src="PM/CAD/fg/10.jpg">
<br> Again go to the "SOLID"- "CREATE"-"FM GEAR" . 
<br>
<img style="float: center;" width=700 src="PM/CAD/fg/12.jpg">
<br> <br> Then Click "Capture Position" .
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/13.jpg">
<br>
Then this interface arrived.
<br<br>

<img style="float: center;" width=700 src="PM/CAD/fg/14.jpg">
<br> There also appared "Sketch Palette" set all needed thing then click "Finish Sketch". 
<br><br>

<img style="float: center;" width=700 src="PM/CAD/fg/15.jpg">
<br>
<br>
Then go to "SOLID " again and then Click "CREATE" then select "Extrude" . 
<img style="float: center;" width=700 src="PM/CAD/fg/16.jpg">
<br><br>
Then this interface open and after select all things click "Ok".
<br> 
<img style="float: center;" width=700 src="PM/CAD/fg/17.jpg">
<br> 
Later, Select "Sketch1" .

<img style="float: center;" width=700 src="PM/CAD/fg/18.jpg">
<br><br>
Then go to "ASSEMBLE" and select "Joint" . 
<img style="float: center;" width=700 src="PM/CAD/fg/19.jpg">
<br> 
<img style="float: center;" width=700 src="PM/CAD/fg/20.jpg">
<br><br>
When click Joint then this interface come. And then Set the "POSITION" and " MOTION " then click "OK". 
<br<br>
<img style="float: center;" width=700 src="PM/CAD/fg/21.jpg">
<br>
Again go to "ASSEMBLE" and select "Joint" for the big gear. 
<img style="float: center;" width=700 src="PM/CAD/fg/22.jpg">
<br<br> 
Then fix the "position" and "Motion" . then click"OK". 

<br>
<img style="float: center;" width=700 src="PM/CAD/fg/23.jpg">
<img style="float: center;" width=700 src="PM/CAD/fg/24.jpg">
<br><br>
 Then go to "ASSEMBLE " again and then select "MOTION" and then set the motion .
<br><br>

Here is our project. 

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e6833968b711a1fe0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


<video width="700" height="500" controls>
  <source src="PM/CAD/fg/FMG.mp4" type="video/mp4">
  <source src="PM/CAD/fg/FMG.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>


