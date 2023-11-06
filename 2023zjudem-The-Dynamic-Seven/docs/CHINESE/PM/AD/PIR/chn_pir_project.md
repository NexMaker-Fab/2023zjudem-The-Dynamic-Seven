
# Arduino带有PIR传感器项目，带有LED和蜂鸣器
<br>
<br>
该项目显示了如何将Arduino与PIR传感器一起自动打开和关闭LED和蜂鸣器。

通过监视附近物体产生的红外（热）辐射量的变化，PIR传感器检测到运动。当检测到运动时，LED将镜头圆顶作为视觉提示。该模块还在其输出引脚上输出一个高信号。
<br>

## **PIR传感器项目Arduino所需的组件**

* Arduino Uno × 1
  <img src="PM\AD\PI\Runo.jpg">
* PIR Sensor × 1 
  <img src="PM\AD\PI\Rpir.jpg">
* Buzzer × 1 
  <img src="PM\AD\PIR\buzzer.jpg">
* LED and Resistor Kit × 1 
  <img src="PM\AD\PIR\led.jpg">
* Breadboard × 1 
  <img src="PM\AD\PIR\board.jpg">
* Jumper wires × 2 
* USB cable type A/B
  

## **软件**

[Arduino IDE](https://www.arduino.cc/en/software)

## **什么是PIR传感器或PIR运动传感器**

PIR传感器Orpir运动传感器是一种电子传感器，可在一定距离内检测红外光的变化，并响应于检测到的IR信号而输出电信号。它们很小，便宜，低功率，易于使用，并且不磨损。结果，它们经常在房屋和企业中使用的电器和小工具中找到。它们也被称为PIR，“被动红外”，“ Pyroelectric”或“ IR运动”传感器。

PIR传感器基本上是由pyroelectric传感器组成的（在下面可以看作是带有矩形晶体的圆金金属），可以检测红外辐射水平。一切都散发出一些辐射，更热的东西会散发出更大的辐射。实际上，在运动探测器中，传感器分为两半。原因是我们尽量不检测运动的平均水平（更改）。两半被连接以取消彼此。那是因为我们试图不检测平均IR运动（变化）水平。两半被连接以相互取消。当辐射的一半或多或少是IR时，输出将高或低摆动。

该传感器具有可控的灵敏度，可允许运动检测范围为3米至7米，其中包括时间延迟更改和选择触发器，以在应用程序中进行微调。


**主要特征：**

* 通常检测到最多30英尺的人，或以低灵敏度模式检测到15英尺的距离。
* 视场约为90度。
* 通过安装2-56个尺寸螺钉的安装孔使其在永久应用中易于集成。
* 圆顶被LED照明为传感器激活的视觉信号。
* 与任何微控制器的通信很简单。
* 3针SIP包装非常适合需要面包板的项目。
* 它的小尺寸使隐藏起来很容易。
<br>

**调整**

* 顺时针调节距离电位器会增加传感距离（约7米），而逆时针降低了感应距离（约3米）。
* 顺时针调整延迟电位器以加长延迟（300s）或顺时针方向以缩短诱导延迟（5s）。

**典型应用:**

* 照明：灯，自动开关，街道照明，运动激活的夜灯
* 防犯罪设备：安全摄像机，预防犯罪传感器，安全灯，夜间安全警报
* 家用电器：空调，空气净化器，风扇加热器
* 音频和视觉设备：电视，PC，显示
* 商业设备：自动售货机，复制机器



**PIR传感器规格**

* 电压5V-12V DC
* 功耗65mA
* PIR传感器范围在7米以内，小于120°
* 角传感器<110°锥角
* 延迟时间5  -  300s（可调）范围（约0.3秒 -  5分钟）
* 锁定时间0.2秒
* 块时间2.5（默认）可以使范围（0.xx至数十秒
* 温度-15°C〜 +70°C
* 触发方法L  - 禁用重复触发，H  - 启用重复触发器
* 尺寸32×24mm


## **带有Arduino，LED和蜂鸣器的PIR传感器电路图**

<img src="PM\AD\PIR\circuit.png">

<br><br>
PIR传感器的引脚连接到数字引脚2。LED通过220OHM电阻从数字引脚4连接到接地。连接到数字PWM（〜）引脚5的蜂鸣器。
<br>
<br>

## **带LED和蜂鸣器的PIR传感器Arduino代码**


    int PIRSensor = 2; //Define PIR Sensor pin
    int Buzzer = 5; //PWM (~) pin
    int LED = 4; //Define LED pin
    int SensorValue = 0; // Initializing the value as zero at the beginning
  
    void setup() {
    pinMode(Buzzer, OUTPUT);
    pinMode(LED, OUTPUT);
    pinMode(PIRSensor, INPUT);
    Serial.begin(9600);
    }

    void loop() {
    SensorValue = digitalRead(PIRSensor); // The value read from PIR Sensor pin 2 will be assigned to 'SensorValue'
    if(SensorValue == HIGH){
      digitalWrite(LED, HIGH); // Turn LED ON
      tone(Buzzer, 5000); //the buzzer sound frequency at 5000 Hz. The frequency range is from 31 Hz to 65535 Hz.
      Serial.println("Motion Detected"); // Print this text in Serial Monitor
    }
    else
    {
      digitalWrite(LED, LOW);
      noTone(Buzzer);
      Serial.println("Motion not Detected");
    }
    }

## **结果**
<br>
 当物体或运动在PIR传感器范围内，LED和蜂鸣器打开。
<br>
<br>
 <video width="700" controls>
  <source src="PM\AD\PIR\pir_video.mp4" type="video/mp4">
  <source src="PM\AD\PIR\pir_video.mp4" type="video/ogg">
您的浏览器不支持视频标签。
</video>
