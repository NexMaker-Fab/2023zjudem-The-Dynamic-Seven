# Here we will make a cardan Joint.

**Tools&Commands**

- Components
- Joints
- Hole
- Extrude(Revolve)
- Combine
- Extrude(Cut)
- Fillet


Here you can see all dimensions.Our basic structure.
<br>
<br>

**Engineering Drawing**
<iframe src="https://myhub.autodesk360.com/ue2fb5969/shares/public/SHd38bfQT1fb47330c99adbcc3338b7aaf0d?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
<br>
<br>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/1.1.1.png">
<BR>

<br>
Select New Design.We can open it from the file option or shortcut "Ctrl+N".
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/2.png">
<BR>
"CTRL+s" Here we can add our model name and save it.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/3.png">
<BR>
For this model, we will use all units in centimetres.From here we changed the unit to centimetre.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/4.png">
<BR>
From the ASSEMBLE option we created new components.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/5.png">
<BR>
Select the new component and from the CREATE option create a new Sketch and select a plane. Here we select the FRONT part.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/6.png">
<BR>
Select Rectangle this time we used a center rectangle. And make rectangle 4,6.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/7.png">
<BR>
From MODIFY Select the Offset Option to make a -1.cm offset.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/8.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/9.png">
<br>
 Click Finish Sketch
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/10.png">
<BR>

**Extrude**
After creating a sketch, select the "Extrude" command from the toolbar or the right-click context menu. You can also find it in the "Create" dropdown menu. Click on the sketch region you want to extrude. The selected area will be highlighted.

Fusion 360 will now display the Extrude dialog box. Here, you can set several parameters:

- Distance: Specify how far you want to extrude the sketch in the third dimension. You can enter a specific value or drag the arrow in the graphics area.

- Direction: Choose whether to extrude in one direction, symmetrically on both sides or to a specific face or plane.

- Operation: You can perform various operations like "Join," "Cut," "Intersect," or "New Body." This determines how the extrusion interacts with existing geometry.

- Taper Angle: If needed, you can add a taper to the extrusion by specifying an angle.

- Start:End: Use these options to specify where the extrusion starts and ends relative to your sketch. These parameters are available if you choose the "New Body" operation.
- Click the "OK" button in the Extrude dialog box to confirm and create the 3D object.
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/11extrude.png">
<BR>
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/11.1.png">
<BR>
Make a new Sketch make two circles in the center of the object.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/12.png">
<BR>
Finish Sketch
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/13.png">
<BR>
Select a small circle, operation the "cut" distance -3.50cm. It will cut the object.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/14.png">
<BR>
Now select the big circle this time join the operation.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/16.png">
<BR>

**Cylinder**

- Choose a plane on which you want to create the cylinder.
- To create a cylinder, go to the "Create" dropdown menu and select "Cylinder" from the "Primitives" section.
- Click on the location in the sketch plane where you want the center of the cylinder's base to be.
- Drag the cursor or input a value to define the diameter of the base of the cylinder.
- Now, you need to specify the height of the cylinder. You can either drag the cursor in the desired direction or enter a specific value.
- After specifying the base center, diameter, and height, click to confirm the cylinder creation.
- Once you're satisfied with your cylinder, finish the feature by clicking "OK" or "Enter" to exit the sketch environment and complete the cylinder.

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/17cylinder.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/18cylinder.png">
<BR>

**Fillet**

- After selecting the object or the edges want to fillet, go to the "Modify" dropdown menu and choose the "Fillet" command.
- Click on the edges or faces you want to round. Fusion 360 will highlight the selected areas.
- In the "Fillet" dialog box, you'll need to specify the fillet radius. This determines how large the rounded region will be. You can either enter a specific value or use the slider to adjust the radius interactively.
-Additional Options (Optional):
Fusion 360 provides additional options in the "Fillet" dialog box, including:

Face Fillet: If you selected faces, you can choose to create a fillet that rounds the entire face.
Multiple Fillets: You can select multiple edges or faces to fillet in one operation.
Symmetric Fillet: Creates a symmetric fillet on an edge.
Tangent Chain: Automatically selects a chain of connected edges or faces to fillet.

As you adjust the fillet parameters, Fusion 360 will provide a live preview of the filleted edges or faces. Ensure the result looks the way you want and click OK.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/19fillet.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/20fillet.png">
<BR>

**Mirror**

- Choose the component or feature that you want to mirror. This can be a sketch, a body, a component, or a feature like a hole, extrusion, or fillet.
- There are a couple of ways to access the Mirror command:

  - Go to the "Create" dropdown menu and select "Mirror" from the "Pattern" section.
  - Right-click on the object you want to mirror in the Fusion 360 graphics area or in the Fusion 360 Browser and select "Mirror" from the context menu.
- There are a couple of ways to access the Mirror command:

- Go to the "Create" dropdown menu and select "Mirror" from the "Pattern" section.
- Right-click on the object you want to mirror in the Fusion 360 graphics area or in the Fusion 360 Browser and select "Mirror" from the context menu.

- In the "Mirror" dialog box, select the components you want to include in the mirroring operation. You can choose the original object, the mirrored object, or both. Make sure to select the appropriate options based on your design needs.
- Fusion 360 will provide a live preview of the mirrored objects and their positions. Ensure that the result aligns with your design intent.
- Once you're satisfied with the preview, click the "OK" button in the "Mirror" dialog box to confirm and apply the mirroring operation.
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/21m.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/22m.png">
<BR>

**COPY**

- Choose the component, feature, sketch, or object that you want to duplicate.
- There are a few ways to access the Copy command:

  - Go to the "Modify" dropdown menu and select "Copy" from the "Move/Copy" section.
  - Right-click on the selected object in the Fusion 360 graphics area or in the Fusion 360 Browser and choose "Copy" from the context menu.
- Fusion 360 will prompt you to specify a reference point. Click on a specific point or edge of the object that will be used as the reference for duplication.
- Click on the location where you want to place the copy of the object. You can either drag the object to the desired location or enter specific coordinates.
- After specifying the copy point, destination point, and any additional settings, click the "OK" button in the "Copy" dialog box to confirm and create the copy.
- Here you can see our second component is a copy of component one.
<br>

<img style="float: center;" width=1000 src="PM/CAD/cad_img/23copy.png">
<BR>
From ASSEMBLE select New Component.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/24new_com.png">
<BR>
Make another Cylinder.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/25make_cylinder.png">
<BR>

**Combine**

- Start by selecting the 3D bodies, components, or features that you want to combine. These can be bodies, components, or features in your design. You can select them directly in the graphics area or from the Fusion 360 Browser.
- Access the Combine command in one of the following ways:
  - Go to the "Modify" dropdown menu and select "Combine" from the "Combine" section.
  - Right-click on one of the selected objects in the Fusion 360 graphics area or in the Fusion 360 Browser, and choose "Combine" from the context menu.

<B>Combine Operation</B>

In the "Combine" dialog box, you'll have the following options for the combine operation:

- Join: This combines the selected objects into a single, merged body.

* Cut: This subtracts the selected objects from one another, creating a cut or void where they intersect.
- Intersect: This keeps only the common areas of the selected objects, discarding the rest.

- "Cut" operation, you'll need to specify the target and tool bodies. The target body is the object you want to cut, while the tool bodies are the objects that will be used to perform the cutting. Fusion 360 will provide a live preview of the result of the combined operation. Make sure the preview matches your design intent. Click OK.

<br>
<img style="float: center;" width=1000 src="PM/CAd/cad_img/26combine.png">
<BR>

Use the fillet option.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/27.png">
<BR>

Make a copy of pin 1 using the Move function. and make pin 2.

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/28.png">
<BR>

**New component**

- Start by opening an existing design or creating a new one in Fusion 360.
- There are a few ways to create a new component:
  - In the Fusion 360 Browser, right-click on the top-level component (usually named "Component1") or an existing component and select "New Component."
  - Go to the "Assembly" dropdown menu and choose "New Component."
Create Empty Component: This option creates an empty component with no geometry. You can then add sketches, bodies, and features to it as needed.
After specifying the component name and choosing the creation method, click the "OK" button to create the new component.

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/29cb.png">
<BR>

**Project**

The "Project" feature is a useful tool for creating reference geometry or capturing 2D sketches on 3D surfaces. It allows you to transfer specific geometry or information from a 3D model to a 2D sketch. Here's how the Project feature works:

There are a few ways to access the Project command:

- In the Sketch workspace, go to the "Create" dropdown menu and select "Project/Include" from the "Insert" section.
- In the sketch environment, right-click on the sketch palette or an existing sketch entity and choose "Project/Include" from the context menu.
- You can click "p" on your keyboard the Project command will run.

Click on the 3D model's edges, faces, or other geometry that you want to project into the current sketch. Fusion 360 will highlight the selected geometry.

After selecting the geometry, you may need to specify the direction in which the projection will occur. Fusion 360 will project the selected geometry perpendicularly to the sketch plane by default. However, you can also set a custom projection direction if needed.

Fusion 360 will project the selected 3D geometry onto your sketch plane. You'll see a live preview of the projected lines and points. Make sure the projection aligns with your design intent.

Once you're satisfied with the projection, click the "OK" button in the "Project" dialog box to confirm and create the sketch entities.
Make pin1 upper part as Project.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/30project.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/31project.png">
<BR>
  
**Sketch Dimension**

Adding dimensions to a sketch in Fusion 360 is an essential step in creating precise and parametric 2D geometry. Here's how to add dimensions to a sketch:

- Start by either creating a new sketch on a specific plane or opening an existing sketch in Fusion 360.
- In the Sketch workspace, select the "Sketch Dimension" tool. You can find it in the "Sketch" dropdown menu or on the toolbar.
- Click on the sketch entities (lines, arcs, circles, etc.) that you want to dimension. Fusion 360 will highlight the selected entities.
- Click on the location where you want to place the dimension. This action will create a dimension line, and the dimension value will appear. You can drag the dimension value to reposition it if needed.
- After placing the dimension, you can either type a specific value on your keyboard or drag the dimension line to set the desired dimension. Fusion 360 will automatically update the sketch geometry to match the new dimension.
- In the Fusion 360 Browser, you'll find the "Sketch Palette." It provides a list of dimensions, constraints, and sketch entities. You can use the Sketch Palette to easily manage and edit your sketch's dimensions and constraints.

Here First select Center Block.
Create a new Sketch.
Select circle.
Make two circles small one with 1 cm dimensions and the second one with 2 cm dimensions.
Select Sketch Dimension.
First, select the project line and then select the circle center and make the vertical distance between them 2 cm and horizontally 1 cm.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/32.png">
<BR>
After finishing the sketch.
Now used the Extrude command.
Select Center Block then select Extrude.
Now select the profile here select 1 cm circle and direction Symmetric. Distance 1.25 cm Operation New Body.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/33cb.png">
<BR>
Now select the extrude command
Select 1cm and 2cm circles at the same time.
Start operation from object.
Distance 1 cm
Select operation 'Join'
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/34cb.png">
<BR>
In the Center Block Select Mirror.
In mirror select the object type "Features"
Select Object that extruded in the center Block
Select the Mirror plane as the Image
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/35cb.png">
<BR>
Now copy and Move.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/36cb.png">
<BR>

Make a New Sketch . Open Project and select the left Circle as Image. Now make a rectangle with 5 cm and 1 cm.
Select Sketch Dimension and make a 0.5 cm distance between the circle center and the rectangle 5cm line.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/37cb.png">
<BR>
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/38cb.png">
<BR>

Now Extrude the selected part.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/39cb.png">
<BR>
Use the Mirror command.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/40.png">
<BR>
Here are our all components.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/41all_com.png">
<BR>
Now we add some additional components that will be our ground.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/42.png">
<BR>
Make a copy and move it.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/43.png">
<BR>
Make Component 4.1 to ground.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/44ground.png">
<BR>

**Joint**

Working on joint designs in Fusion 360 involves creating connections and relationships between components or bodies in your 3D model to simulate how they move and interact with one another. Joints are essential for designing assemblies, especially if you want to test how parts fit together and how they move before manufacturing. Here's a basic overview of how to work with joints in Fusion 360:

Make sure you have multiple components or bodies in your design that you want to connect using joints. If you don't, you may need to create additional components.

Activate the Joint Tool:

Click on the "Assemble" workspace in the toolbar to access assembly tools.
Select the "Joint" command from the "Assemble" menu.

Select Components: Use the "Select" tool to choose the components or bodies you want to join together. Typically, you select two components to define a joint.

Choose the Joint Type: Fusion 360 offers various types of joints to simulate different types of motion. Some common joint types include:

Revolute Joint: Simulates rotational motion, like a hinge or pivot.
Slider Joint: Simulates linear motion, like a sliding drawer.
Cylindrical Joint: Combines both translational and rotational motion.
Planar Joint: Constrains components to move in a plane, like a sliding door.
Ball Joint: Allows for rotational motion around multiple axes, like a ball and socket joint.

Configure Joint Parameters: Depending on the type of joint you selected, Fusion 360 will ask you to define parameters. This could include specifying the axis of rotation for a revolute joint, the direction of linear motion for a slider joint, or other relevant parameters.

Test the Assembly: After creating joints, you can use the "Motion Study" feature to test how the components move and interact. This can help you ensure your design works as intended.

Here First select one component and the ground one.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/45j.png">
<BR>

Here we can see after joint.

<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/46.png">
<BR>

Now join Pin and Yoko.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/47.png">
<BR>

Check the Motion.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/48j.png">
<BR>

Now join pin and Center Block
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/49j.png">
<BR>

Adjust the pin and Center Block position.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/50j.png">
<BR>
Select another pin and Center Block and join them.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/51.png">
<BR>
Adjust Position.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/52.png">
<BR>
Now select Yoko and the pin. And join them.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/53.png">
<BR>
Join the Yoko
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/54.png">
<BR>
Now we can see all components join.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/55all.png">
<BR>
Now set the moving rotation. Click M on keyboard and at first select Yoko 1 and then select the pin. After selecting the pin again unselect the Yoko. Now adjust the pin in z angle to 22.5 degrees.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/56.png">
<BR>

After adjusting the degree here is our final 3D model.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/57final.png">
<BR>
For a better view hide Component 4.1 and Component 4.2.
Go joints file here and click the right button in Mouse in Revolute 6. and Select Animate Joint Relationship.
Now we can see our final Model.
<br>
<img style="float: center;" width=1000 src="PM/CAD/cad_img/58.png">
<BR>

**Appearance**

Using the "Appearance" feature in Fusion 360, you can apply various visual properties to your 3D models to make them look more realistic. These appearances can simulate the way materials and finishes appear in the real world. Here's how to use appearances in Fusion 360:

In the toolbar, click on the "Appearance" icon, which looks like a paint bucket.

In the Appearance panel, you can browse a library of predefined appearances. You can choose from materials like wood, metal, plastic, glass, and more. There is a wide range of options available.

To apply an appearance to a part of your model, select the part by clicking on it in the workspace or selecting it from the model tree.
Once the part is selected, choose the appearance you want from the Appearance panel by clicking on it.

After applying an appearance, you can customize it further. Click the appearance in the Appearance panel, and you'll see options to adjust properties like color, gloss, bump, and transparency.

You can make materials transparent by adjusting the transparency slider.

If you create a custom appearance that you want to reuse in the future, you can save it as a custom appearance.
Apply Appearances to Different Parts:

You can apply different appearances to different parts of your model to simulate different materials and finishes.
Render Your Model:

To see the appearance in its full glory, you can use Fusion 360's rendering capabilities. This will give you a photorealistic representation of your model with the applied appearances.
Save and Export:

After you're satisfied with the appearance, save your model and export it in the desired format for presentation or manufacturing.
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




## How to add project to our website from [Myhub Autodesk360](https://myhub.autodesk360.com/)

1. Open Fusion 360 in our machine and select our project.At first check your offline or online.If offline select online.
<br>

<img style="float: center;" width=1000 src="PM/CAD/add_1.png">
<BR>
2. Click on Data Panel then click  Open on the web.
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_2.png">
<BR>
3. Click on your project.
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_3.png">
<BR>
4. Click on Shared link and turn on it.
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_4.png">
<BR>
5. Select Embed and copy the link .
<br>
<img style="float: center;" width=1000 src="PM/CAD/add_5.png">
<BR>

6. Past the link on the website.

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

7. We add gif with this code

         <BR>
         <img style="float: center;" width=1000 src="PM/CAD/afra.gif">
         <BR>
