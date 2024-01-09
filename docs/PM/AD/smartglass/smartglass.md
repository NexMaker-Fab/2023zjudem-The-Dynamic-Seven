# Title: InclusiveVision - Smart Glasses for Visually Impaired Individuals

This are the smart glasses which can tell you about how much far/near the object is in front of you. Helpful for blind people.

**Components and supplies**
<br>

* Ultrasonic Sensor - HC-SR04 (Generic)
* Arduino UNO
* Jumper wires (generic)
<br>

**Project description**
This works as in the ultrasonic sensor which is mounted on the head of the glasses, constantly keeps on detecting the objects in front of them, and sends an alert system through headphones.

**Circuit diagram**
<br>
<img src="PM\AD\smartglass\circuit_diagram.png" style="float: center;" width=800 height=700 >
<br>

**Code**

```
#define TRIG_PIN 6
#define ECHO_PIN 5
#define BUZZER_PIN 7

void setup() {
  pinMode(TRIG_PIN, OUTPUT);
  pinMode(ECHO_PIN, INPUT);
  pinMode(BUZZER_PIN, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  // Trigger ultrasonic sensor
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  // Read the echo pulse duration
  long duration = pulseIn(ECHO_PIN, HIGH);

  // Calculate distance in centimeters
  int distance = duration * 0.034 / 2;

  // Provide feedback based on distance
  if (distance < 50) {
    // Obstacle detected
    tone(BUZZER_PIN, 1000); // Activate buzzer
  } else {
    // No obstacle
    noTone(BUZZER_PIN); // Deactivate buzzer
  }

  Serial.println(distance); // Print distance for debugging

  delay(100); // Adjust delay as needed
}
```

**Result** 

<br>
<img src="PM\AD\smartglass\r1.jpg" style="float: center;" width=800 height=700 >
<br>

<br>
<img src="PM\AD\smartglass\r3.jpg" style="float: center;" width=800 height=700 >
<br>

<br>

<video width="720" height="540" controls>
<source src="PM\AD\smartglass\r2.mp4" type="video/mp4">
<source src="PM\3D_print\w_1.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
<br>

