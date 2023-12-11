## Control Arduino Using Processing

<br> 

## Hardware components

* Arduino
* Breadboard (generic)	
* LED
* 240 Ohm Resistor
* Jumper wires◊

<br>

## Software apps and online services
* Arduino IDE
* Processing

## What is Processing?
<br>
Processing is a flexible software sketchbook and a language for learning how to code within the context of the visual arts. Processing is very useful platform for hobbyists, researchers, students for learning and prototyping. Some of the features are:

1. Free and open source
2. For all platforms (GNU/Linux, Mac OS X, Windows, Android, and ARM)
3. Well documented
4. Many libraries
5. Good community
6. Arduino IDE
   
<br>

**Processing IDE**

To download Processing go here: [Processing Download](https://processing.org/download)


<br>
<img src="PM/IPA/led/pic1.jpg"style="float: center;" width=700 height=500 >
<br>
<br>
<img src="PM/IPA/led/pic2.jpg" style="float: center;" width=700 height=500 >
<br> 

There are many libraries for different applications. You can also install some extra libraries manually or directly from the menu.

To install new library from menu, go to: Sketch -> Import Library... -> Add Library...

<br>
<img src="PM/IPA/led/pic3.jpg" style="float: center;" width=700 height=500 >
<br> 

But at the moment we are interested only in GUI design. And there is a very nice library called ControlP5 is available to create our project. controlP5 is a library written by Andreas Schlegel for the programming environment Processing. To add ControlP5 library to Processing just follow the add library process and search for ControlP5 and then click on install. Now you are ready to create your GUI application.

<br>
<img src="PM/IPA/led/pic4.jpg" style="float: center;" width=700 height=500 >
<br> 

Once you have installed ControlP5, start with creating simple window. See the video down below to get basic idea how to create window and add buttons to the window.
Next step is to write a Arduino sketch. Write a code in such a way that when Arduino receives any character over serial port, it performs some particular task. For example

```
     if(val == 'r'){           //if r received 
     digitalWrite(11, HIGH); //turn on pin 11 (red led in our case) 
     } 
```

So when Arduino receives char 'r', it sets pin 11 to High. Please check the codes in code section below to get exact idea.Now comes the Processing part. There is a Serial library in the Processing and we can use that to read and write to the serial port. So what we do now is we assign a function to each of the buttons to send some character to serial port, so when you press any button, it send particular char to the serial port. For example suppose we have a button called red, when you press button red it sends char 'r' to the serial port.

 ```
    void red(){ 
    port.write('r'); 
    } 
 ```   

 At the other end, Arduino receives that char 'r' and according to the received char it changes state of the pins.
Please check the code, so you can get exact idea how to add buttons and assign functions to the buttons.Code is in the Code section. There you will find code for both, Arduino and Processing. First compile and upload the Arduino sketch to the arduino and then run Processing sketch.

## Components and Circuit

<br>
<img src="PM/IPA/led/pic5.jpg" style="float: center;" width=700 height=500 >
<br> 

Processing window will be look like following if you use code provided below.
<br>
<img src="PM/IPA/led/pic6.jpg" style="float: center;" width=700 height=500 >
<br> 

## Code

**Arduino Code**

```


  void setup() {
  pinMode(10, OUTPUT);   
  pinMode(11, OUTPUT);  
  pinMode(12, OUTPUT);
  pinMode(13, OUTPUT);

  Serial.begin(9600);    //start serial communication @9600 bps
  }

void loop(){
  
  if(Serial.available()){  //id data is available to read

    char val = Serial.read();

    if(val == 'r'){       //if r received
      digitalWrite(11, HIGH); //turn on red led
      }
    if(val == 'b'){       //if b received
      digitalWrite(10, HIGH); //turn on blue led
      }
    if(val == 'y'){       //if y received
      digitalWrite(12, HIGH); //turn on yellow led
      }
     if(val == 'w'){       //if w received
      digitalWrite(13, HIGH); //turn on yellow led
      }
    if(val == 'f'){   
      digitalWrite(13, LOW);//if f received
      digitalWrite(11, LOW); //turn off all led
      digitalWrite(12, LOW);
      digitalWrite(10, LOW);
      
      }      
    }
  }

```

**Processing code**

```
import controlP5.*; //import ControlP5 library
import processing.serial.*;

Serial port;

ControlP5 cp5; //create ControlP5 object
PFont font;

void setup(){ //same as arduino program

  size(300, 450);    //window size, (width, height)
  
  printArray(Serial.list());   //prints all available serial ports
  
  port = new Serial(this, "COM3", 9600);  //i have connected arduino to com3, it would be different in linux and mac os
  
  //lets add buton to empty window
  
  cp5 = new ControlP5(this);
  font = createFont("calibri light bold", 20);    // custom fonts for buttons and title
  
  cp5.addButton("red")     //"red" is the name of button
    .setPosition(100, 50)  //x and y coordinates of upper left corner of button
    .setSize(120, 70)      //(width, height)
    .setFont(font)
  ;   

  cp5.addButton("yellow")     //"yellow" is the name of button
    .setPosition(100, 150)  //x and y coordinates of upper left corner of button
    .setSize(120, 70)      //(width, height)
    .setFont(font)
  ;

  cp5.addButton("blue")     //"blue" is the name of button
    .setPosition(100, 250)  //x and y coordinates of upper left corner of button
    .setSize(120, 70)      //(width, height)
    .setFont(font)
  ;
  
  cp5.addButton("alloff")     //"alloff" is the name of button
    .setPosition(100, 350)  //x and y coordinates of upper left corner of button
    .setSize(120, 70)      //(width, height)
    .setFont(font)
  ;
}

void draw(){  //same as loop in arduino

  background(150, 0 , 150); // background color of window (r, g, b) or (0 to 255)
  
  //lets give title to our window
  fill(0, 255, 0);               //text color (r, g, b)
  textFont(font);
  text("LED CONTROL", 80, 30);  // ("text", x coordinate, y coordinat)
}

//lets add some functions to our buttons
//so whe you press any button, it sends perticular char over serial port

void red(){
  port.write('r');
}

void yellow(){
  port.write('y');
}

void blue(){
  port.write('b');
}

void alloff(){
  port.write('f');
}
```

## Result
<br>
<img src="PM/IPA/led/pic7.jpg" style="float: center;" width=700 height=500 >
<br> 

<br>
<video width="700" height="500" controls>
  <source src="PM/IPA/led/vdo.mp4" type="video/mp4">
  <source src="PM/IPA/led/vdo.ogg" type="video/ogg">
</video>
<br>

