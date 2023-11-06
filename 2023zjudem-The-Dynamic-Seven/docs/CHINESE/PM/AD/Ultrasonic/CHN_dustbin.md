# 聪明的垃圾箱 Smart Dustbin
<br>
<br>
Smart Dustbin的名字巧妙地代表了其工作，或者我们可以说这是一个自动垃圾箱。我们可能会得出结论，这是使您的房屋整洁和吸引人的好设备。儿童主要是通过纸，说唱歌手和其他各种物品分发废物。他们会玩这个垃圾箱时，他们会非常享受自己，并且在玩游戏时，他们也会清理您的房屋，因为聪明的垃圾箱每次使用时都会吸引孩子们。通常，它们将被用来清空所有废物并将其垃圾倒入这个聪明的垃圾箱中。如果您的手充满了垃圾或混乱，则可以手动打开它，可以使用这种情况。甚至蚊子也不会移动，因为它会自动打开而不会触摸，这可以帮助阻止冠状病毒的传播。
<BR><BR>

## 组件要求

* Arduino UNO<br>
<img src="PM\AD\Ultrasonic\uno.jpg">

* Jumper Wires<br>
* Servo Motor<br>
<img src="PM\AD\Ultrasonic\servo.jpg">

* Ultrasonic Sensor<br>
<img src="PM\AD\Ultrasonic\ultrasound.jpg">


## **软件**

[Arduino IDE](https://www.arduino.cc/en/software)

## **Project Hardware Software Selection**
## **项目硬件软件选择**

**Arduino UNO:** 如您所知，Arduino是一个基于微控制器的开源电子原型制作板，可以使用易于使用的Arduino IDE进行编程。UNO是Arduino家族中最受欢迎的董事会之一，也是初学者的绝佳选择。

**Ultrasonic Sensor:** 这些传感器使用超声波来检测对象或测量自己与物体之间的距离。

<span style="color:red">关联 :</span>

[什么是超声波传感器：工作原理和应用](https://robocraze.com/blogs/post/what-is-ultrasonic-sensor)

**Servo Motor:** 这是一种可以推动或拉动的电气设备，还可以精确地旋转对象。如果要以某种特定角度或距离旋转对象，则使用伺服电机。它由一个简单的电动机组成，该电动机通过伺服机构运行。我们可以在小且重量轻的包装中获得很高的扭矩伺服电动机。

<span style="color:red">关联:</span>

[伺服电机：图，定义，类型，工作和应用](https://www.theengineerspost.com/servo-motor/)



## **电路原理图**

<img src="PM\AD\Ultrasonic\circuit.png" >

## **Code**

    #include <Servo.h>   //servo library
    Servo servo;
    int trigPin = 5;
    int echoPin = 6;  
    int servoPin = 7;
    int led= 10;
    long duration, dist, average;  
    long aver[3];   //array for average
    void setup() {
        Serial.begin(9600);
        servo.attach(servoPin);
        pinMode(trigPin, OUTPUT);
        pinMode(echoPin, INPUT);
        servo.write(0);         //close cap on power on
        delay(100);
        servo.detach();
    }
    void measure() {
     digitalWrite(10,HIGH);
    digitalWrite(trigPin, LOW);
    delayMicroseconds(5);
    digitalWrite(trigPin, HIGH);
    delayMicroseconds(15);
    digitalWrite(trigPin, LOW);
    pinMode(echoPin, INPUT);
    duration = pulseIn(echoPin, HIGH);
    dist = (duration/2) / 29.1;    //obtain distance
    }
    void loop() {
      for (int i=0;i<=2;i++) {   //average distance
        measure();
       aver[i]=dist;
        delay(10);              //delay between measurements
      }
     dist=(aver[0]+aver[1]+aver[2])/3;
    if ( dist<50 ) {
    //Change distance as per your need
     servo.attach(servoPin);
      delay(1);
     servo.write(0);
     delay(3000);
     servo.write(150);
     delay(1000);
     servo.detach();
    }
    Serial.print(dist);
    }


## **结果**


<img src="PM\AD\Ultrasonic\img 2.png">

<video width="700" controls>
  <source src="PM\AD\Ultrasonic\video.mp4" type="video/mp4">
  <source src="PM\AD\Ultrasonic\video.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
