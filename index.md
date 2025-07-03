# Cardboard Robot
<!---Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails! --->
<!---
You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:--->
 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->


| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Mihika K | Los Altos High School | Mechanical/Electrical Engineering | Incoming Junior

<!---**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.** --->

![Headstone Image](logo.svg)
  
# Final Milestone

<!---**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE --->

<iframe width="560" height="315" src="https://www.youtube.com/embed/0KXFxS0ANo4?si=rPcJuxnakEG7SYnT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Description:**
In this milestone, I put together the cardboard body of the robot with its electrical circuit. This circuit includes 2 RGB LEDs, 5 servos controlling the motion of the limbs and head, and 2 sensors: an Ultrasonic Sensor and a Microphone. The robot has three modes, 1) when the Ultrasonic Sensor is activated, 2) when the microphone is activated, and 3) when neither sensor is activated. In the first mode, the Ultrasonic Sensor detects that an object is within 50 centimeters of the robot and responds with red flashing eyes, and sweeping arms. In the second mode, the Microphone detects a sound of significant volume and responds with blue flashing eyes and sweeping arms. In the third mode, the robot is static, with eyes shifting from purple to blue to pink to off.

**Status:**
Each of the components are wired and soldered into the PBC board, and attached to the Arduino Uno. The sensors are activated by excessive sound and proximity, and in turn activate the servos and LED eyes.

**Challenges and Triumphs:**
The biggest challenge I faced at BSE was the problem of getting the robot to walk. In order to allow the robot mobility in its legs, the robot leg was shaped with a semicircle at the top (as shown in the Robot Net). Although it did ensure movement, it also reduced the robot's stability, due there now being only 4 points of contact that balanced the robot's body. When the robot lifted its leg to walk, it furthered reduced stability. In effort to increase its stability, I added a back brace that would ideally increase stability, and take weight off the robot's legs. Although the back brace did increase stability, it also restricted the robot's ability to walk. 

I'm proud of my work on connecting the sensors to the robot's movements. These sensors allow the robot to be an interactive scarecrow, that sensed external factors and move its limbs in response to them. 

**Summary**
During my time working on the Cardboard RObot, I learned how to construct circuits, considering which components needed a resistor, as well as how Analog and Digital (and PWM) pins worked. I also learned how to code the Arduino and use its libraries (Servo and Ultrasonic) to my advantage. In the future I hope to continue building projects like this one, involving firmware and software to solve small problems.


# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/BYNdLccMI3A?si=dTXreLQWzvdTvkyW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Description:**
For this milestone, I have implemented the sensors that will be part of the final Cardboard Robot. Originally, I had intended to make the robot walk, but due to the weight and problems with the robot's balance, I pivoted to adding sensors so the robot can respond to outside inputs. The circuit in the video demonstrates the usage of the Ultrasound Sensor, and the Microphone. The Ultrasound Sensor works by emitting a frequency of 40 kHz, and measuring the time it takes for the sound to be echoed back. Using the speed of sound, it estimates the distance it is from an object. Note that the speed of sound is about 343 m/s, meaning that this measurement is quite accurate for most moving objects (only planes and rockets can break Mach 1, and they're irrelevant for this project). The Microphone works with two outputs, digital and analog, allowing the analysis of the exact volume, as well as whether there is a significant sound or not.

**Status:**
In this particular circuit, the lightbulbs turn on in response to the sensors (red turns on when the Ultrasound Sensor detects an object between 10 and 30 centimeters from it, blue turns on if it detects an object within 10 centimeters, and green turns on in response to a lound sound). Although these lightbulbs won't be in the final robot, the robot will have its own reactions to external stimuli.

**Challenges:**
This milestone required me to consider the specifications of the Ultrasound Sensor, and the Microphone, which I had never used before. The microphone particularly didn't have a lot of documentation online, so I brainstormed how I could analyze the Analog output to differentiate sounds of different levels. By adjusting its sensitivity, I set the microphone so that it could hear detect a person talking.

**Plan:**
I plan on integrating these sensors with the larger robot, so that he can respond to inputs from these sensors. In addition I plan on completing and soldering the circuits.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Wh0m6Htr8E8?si=Qizf5hZY_ph8THIY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Sensors Schematic
![Headstone_Image](SensorsConfiguration.png)
## Sensors Information
![Headstone_Image](UltrasonicSensor.png)

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/EciZOCs-LQc?si=4pNSvlZnDVBJJbzE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Description:**
The Smartphone Cardboard Robot is built with servos, LEDs, an electrical circuit, and encased with cardboard blocks. Each of the servos allow the movement of the head, the arms, and legs. LEDs in the head simulate eyes, and will blink in different patterns to indicate different modes. The nets and movement models explain the structure of each cardboard limb as well as the body of the robot. As part of this milestone, I tested the servos and their ability to move the cardboard limbs (see schematics and diagrams below).

**Status:**
As of the first milestone, I have completely built the robot's cardboard body, as well as positioned and attached all the servos. This includes considering movement of the robot's limbs and modifying parts of the body to allow for that. For example, the are actually attached to the body with a semicircle shape at the top allowing it to rotate easily.

**Challenges:**
One challenge I'm facing is the robot's stability. While modifying the legs allowed the robot to actually move its legs, it dramatically reduced the robot's stability due to there only being one point of contact between the legs and the body. Another challenge is considering the placement of the electrical circuit so the robot does not topple.

**Plan:**
Later on, I plan to complete the circuit of the robot with the LEDs, and code the app on the smartphone to control the robot. In addition, I plan on adding a motion sensor and sound sensor so that the robot moves towards motion, and stops at sounds above a certain decibel value.

## Robot Net
![Headstone Image](CharlieBuild.png)
## Servos Schematic
![Headstone_Image](ServosConfiguration.png)

# Starter Project: RGB Slider

<iframe width="560" height="315" src="https://www.youtube.com/embed/rhV8uBoarpk?si=_rZ5P_-N4F-b0jgd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
**Description:**
The RGB Slider uses three sliders and a lightbulb. Each of the sliders sends an integer value to the lightbulb to determine the color it displays. This is powered with the USB-C plug on the circuit board. Through this project I intended to practice soldering and understand circuits.

**Challenges:**
I intially had problems with the orientation of the lightbulb, since I had placed the negative end in the wrong pin. This meant the circuit didn't work. When I tried to desolder the lightbulb from the circuit board, I was unable to do so, and instead started over from the beginning.

**Summary:**
This project taught me how to build circuits. In addition, I was able to practice soldering, as well as how to check for short circuits with a multimeter and prevent or remove them.

<!---
# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code

Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 
```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/) --->
## Code for Sensors and Servos (Milestone 3)
```c++
#include <Servo.h>;
#include <HCSR04.h>;
const int LL_PIN = 2;
const int RL_PIN = 8;
const int RA_PIN = 7;
const int LA_PIN = 12;
const int HEAD_PIN = 13;
Servo ll;
Servo la;
Servo rl;
Servo ra;
Servo head;

const int TRIG = 9;
const int ECHO = 5;
float duration, distance;
int sigDistance = 50;
HCSR04 us(TRIG, ECHO);

int micAnalog = A0;
int micDig = 3;
float analogVoltage;

const int PIN_RED = 11;
const int PIN_GREEN = 10;
const int PIN_BLUE = 6;
const int COLOR_INTERVAL = 2000;
int r = 0;
int g = 0;
int b = 0;

int modeRed = 1;
int modeBlue = 2;
int modeHappy = 3;
int ledMode = 0;

bool flagUSsensor = false;
int twelveCycle = 0;
int flag = 0;

unsigned long uSsensorMillis = 0.0;
unsigned long prevMillisColor = 0.0;
unsigned long millisMovement = 0.0;

void setup() {
  ll.attach(LL_PIN);
  la.attach(LA_PIN);
  rl.attach(RL_PIN);
  ra.attach(RA_PIN);
  head.attach(HEAD_PIN);  
  pinMode(micAnalog, INPUT);
  pinMode(micDig,    INPUT);
  pinMode(TRIG,      OUTPUT);
  pinMode(ECHO,      INPUT);
  pinMode(PIN_RED,   OUTPUT);
  pinMode(PIN_GREEN, OUTPUT);
  pinMode(PIN_BLUE,  OUTPUT);

  Serial.begin(9600);
  calibrateServos();
}

void loop() {
  unsigned long currentMillis = millis();
  // Ultrasound Regulation
    distance = us.dist();
    delay(60);
    if (distance < sigDistance){
      Serial.println("FIGHT");
      flag = 1;
      setLED(modeRed);
      sweepArms();
    } else {
      setLED(3);
      flag = 0;
    }

  //mic section
  analogVoltage = analogRead(micAnalog) * (5.0/1023.0);
  Serial.print("Analog Voltage Value: ");
  Serial.println(analogVoltage);
  //refactor for continuous array avgs?
  if (analogVoltage > 0.22 &&  flag != 1){
    r = 0;
    g = 0;
    b = 0;
    setLED(2);
    // if (head.read() != 45){
    //   head.write(45);
    // }
    sweepArms();
  } else {
    if (head.read() != 90){
      head.write(90);
      setLED(3);
    }
  }
  
  //color section
  if (currentMillis - prevMillisColor >= COLOR_INTERVAL){
    prevMillisColor = currentMillis;
    if (ledMode == 0){
      ledMode = 3;
    }
    colorChange(r, g, b);
  }
}

void calibrateServos(){
  ll.write(90);
  rl.write(90);
  ra.write(0);
  la.write(180);
  //head.write(90);
}

void sweepArms(){
  for (int i = 0; i < 4; i++){
    ra.write(180);
    la.write(0);
    delay(500);
    ra.write(0);
    la.write(180);
    delay(500);
  }
  calibrateServos();
}

void redMode(int red, int green, int blue){
  if (red == 0 && green == 0 && blue == 0){
    r = 232;
    g = 33;
    b = 0;
  } else if (red == 232 && green == 33 && blue == 0){
    r = 164;
    g = 16;
    b = 0;
  } else if (red == 164 && green == 16 && blue == 0){
    r = 171;
    g = 255;
    b = 0;
  } else if (red == 171 && green == 255 && blue == 0){
    r = 205;
    g = 0;
    b = 255;
  } else if (red == 205 && green == 0 && blue == 255){
    r = 0;
    g = 0;
    b = 0;
  }
  
  analogWrite(PIN_RED, r);
  analogWrite(PIN_GREEN, g);
  analogWrite(PIN_BLUE, b);
}

void blueMode(int red, int green, int blue){
  if (red == 0 && green == 0 && blue == 0){
    r = 51;
    g = 51;
    b = 255;
  } else if (red == 51 && green == 51 && blue == 255){
    r = 153;
    g = 153;
    b = 255;
  } else if (red = 153 && green == 153 && blue == 255){
    r = 153;
    g = 255;
    b = 255;
  } else {
    r = 0;
    g = 0;
    b = 0;
  }
  analogWrite(PIN_RED, r);
  analogWrite(PIN_GREEN, g);
  analogWrite(PIN_BLUE, b);
}

void happyMode(int red, int green, int blue){
  if (red == 0 && green == 0 && blue == 0){
    r = 255;
    g = 228;
    b = 51;
  } else if (red == 255 && green == 228 && blue == 51){
    r = 255;
    g = 158;
    b = 177;
  } else if (red == 255 && green == 158 && blue == 177){
    r = 102;
    g = 255;
    b = 255;
  } else{
    r = 0;
    b = 0;
    g = 0;
  }
  analogWrite(PIN_RED, r);
  analogWrite(PIN_GREEN, g);
  analogWrite(PIN_BLUE, b);
}

void setLED(int mode){
  ledMode = mode;
}

void colorChange(int red, int green, int blue){
  if (ledMode == modeRed){
    redMode(red, green, blue);
  } else if (ledMode == modeBlue){
    blueMode(red, green, blue);
  } else if (ledMode == modeHappy){
    happyMode(red, green, blue);
  } else {
    r = 0;
    g = 0;
    b = 0;
    analogWrite(PIN_RED, r);
    analogWrite(PIN_BLUE, b);
    analogWrite(PIN_GREEN, g);
  }
}

float findDistance(float duration){
  return duration * (0.0343/2);
}
```
## Code for Servo Testing (Milestone 2)
```c++
#include <Servo.h>

const int LL_PIN = 2;
const int LA_PIN = 4;
const int RL_PIN = 7;
const int RA_PIN = 8;
const int HEAD_PIN = 12;
Servo leftLeg, leftArm, rightArm, rightLeg, head;

void setup() {
  leftLeg.attach(LL_PIN);
  leftArm.attach(LA_PIN);
  rightLeg.attach(RL_PIN);
  rightArm.attach(RA_PIN);
  head.attach(HEAD_PIN);
  reset();
  }

void loop() {
  leftLeg.write(180);
  delay(1000);
  rightLeg.write(0);
  delay(1000);
  leftArm.write(90);
  delay(1000);
  rightArm.write(90);
  head.write(180);
  delay(1000);
  reset();
}

void reset(){
  leftLeg.write(90);
  rightLeg.write(90);
  leftArm.write(0);
  rightArm.write(180); //due to configuration of motors
  head.write(90);
}

```

## Code for Sensor Testing (Milestone 1)
```c++
const int TRIG = 9;
const int ECHO = 6;
const int REDPIN = 13;
const int GREENPIN = 8;
const int BLUEPIN = 12;
int micAnalog = A0;
int micDig = 2;

float analogVoltage;
int digValue;
float duration, distance;

unsigned long prevMillisLow = 0;
unsigned long prevMillisHigh = 0;

void setup() {
  pinMode(micAnalog, INPUT);
  pinMode(micDig, INPUT);
  pinMode(TRIG, OUTPUT);
  pinMode(ECHO, INPUT);
  Serial.begin(9600);
  digitalWrite(REDPIN, LOW);
  digitalWrite(BLUEPIN, LOW);
  digitalWrite(GREENPIN, LOW);
}

void loop() {
  unsigned long currentMillis = millis();
  digitalWrite(TRIG, LOW);
  //replacement for delay-- (2 milliseconds)
  if (currentMillis - prevMillisLow >= 2) {
    prevMillisLow = currentMillis;
    digitalWrite(TRIG, HIGH);
  }
  //replacement for delay-- (10 milliseconds)
  if (currentMillis - prevMillisHigh >= 10) {
    prevMillisHigh = currentMillis;
    digitalWrite(TRIG, LOW);
    duration = pulseIn(ECHO, HIGH);
    distance = (duration*.0343)/2;
    Serial.print("Distance: ");  
	  Serial.println(distance); 

    if (distance < 10){
      digitalWrite(BLUEPIN, HIGH);
      digitalWrite(REDPIN, LOW);
    } else if (distance < 30){
      digitalWrite(REDPIN, HIGH);
      digitalWrite(BLUEPIN, LOW);
    } else {
      digitalWrite(REDPIN, LOW);
      digitalWrite(BLUEPIN, LOW);
    }
  }

  analogVoltage = analogRead(micAnalog) * (5.0/1023.0);
  digValue = digitalRead(micDig);
  Serial.print("Analog Voltage Value: ");
  Serial.println(analogVoltage);
  if (analogVoltage > 0.20){
    digitalWrite(GREENPIN, HIGH);
  } else {
    digitalWrite(GREENPIN, LOW);
  }
}
```
