## 使用处理控制 Arduino
<br> 

＃＃ 硬件组件

* Arduino
* Breadboard (generic)	
* LED
* 240 Ohm Resistor
* Jumper wires◊

<br>

## 软件应用程序和在线服务
* Arduino IDE
* Processing

## 什么是处理？
<br>
Processing 是一本灵活的软件速写本，也是一种用于学习如何在视觉艺术背景下进行编码的语言。对于业余爱好者、研究人员、学生来说，Processing 是一个非常有用的学习和原型制作平台。其中一些功能是：

1. 免费开源
2. 适用于所有平台（GNU/Linux、Mac OS X、Windows、Android 和 ARM）
3. 有据可查
4.很多图书馆
5.良好的社区
6.Arduino集成开发环境
<br>


**处理IDE**

要下载处理，请转到此处：[Processing Download](https://processing.org/download)


<br>
<img src="PM/IPA/led/pic1.jpg"style="float: center;" width=700 height=500 >
<br>
<br>
<img src="PM/IPA/led/pic2.jpg" style="float: center;" width=700 height=500 >
<br> 

有许多用于不同应用的库。您还可以手动或直接从菜单安装一些额外的库。

要从菜单安装新库，请转到：Sketch -> Import Library... -> Add Library...

<br>
<img src="PM/IPA/led/pic3.jpg" style="float: center;" width=700 height=500 >
<br> 

但目前我们只对 GUI 设计感兴趣。有一个非常好的库，称为 ControlP5，可用于创建我们的项目。 controlP5是Andreas Schlegel为编程环境Processing编写的一个库。要将 ControlP5 库添加到处理中，只需按照添加库过程并搜索 ControlP5，然后单击安装即可。现在您已准备好创建 GUI 应用程序。

<br>
<img src="PM/IPA/led/pic4.jpg" style="float: center;" width=700 height=500 >
<br> 

安装 ControlP5 后，开始创建简单的窗口。请观看下面的视频，了解如何创建窗口并向窗口添加按钮的基本概念。
下一步是编写 Arduino 草图。以这样的方式编写代码，当 Arduino 通过串行端口接收到任何字符时，它会执行一些特定的任务。例如

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

## 元件和电路

<br>
<img src="PM/IPA/led/pic5.jpg" style="float: center;" width=700 height=500 >
<br> 

如果您使用下面提供的代码，处理窗口将如下所示。
<br>
<img src="PM/IPA/led/pic6.jpg" style="float: center;" width=700 height=500 >
<br> 
＃＃ 代码

**Arduino代码**

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

**处理代码**

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

＃＃ 结果
<br>
<img src="PM/IPA/led/pic7.jpg" style="float: center;" width=700 height=500 >
<br> 

<br>
<video width="700" height="500" controls>
  <source src="PM/IPA/led/vdo.mp4" type="video/mp4">
  <source src="PM/IPA/led/vdo.ogg" type="video/ogg">
</video>
<br>

