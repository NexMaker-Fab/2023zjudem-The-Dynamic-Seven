
### Plugin
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