# Arduino Sonar Scanner

I built this project to explore how sensors and actuators can work together in real time.  
Using an **ultrasonic sensor mounted on a servo motor**, the system sweeps from 0° to 180° and back, measuring distances just like a radar.

## 🎮 How It Works
- The **servo motor** rotates the ultrasonic sensor to scan the surroundings.  
- The sensor measures distance and provides live feedback.  
- Depending on how close an object is, LEDs and a buzzer indicate the status:  
  - 🟢 **Green LED** → Safe (distance > 40 cm)  
  - 🔵 **Blue LED + slow buzzer** → Warning (10–40 cm)  
  - 🔴 **Red LED + fast buzzer** → Danger (< 10 cm)  

This gives a simple radar-like system that responds to the environment in real time.

---

## ✨ What I Learned
Through this project, I practiced:
- Controlling a **servo motor** for scanning motion  
- Taking **input from an ultrasonic sensor**  
- Driving **output devices** (LEDs and buzzer) based on distance  
- Combining everything into a working system with Arduino  

---

## 🛠️ Components
- 1 × Arduino Uno (or compatible board)  
- 1 × Ultrasonic Sensor (HC-SR04)  
- 1 × Servo Motor (SG90 or similar)  
- 3 × LEDs (Red, Green, Blue)  
- 1 × Buzzer  
- Resistors (220Ω for LEDs)  
- Breadboard + jumper wires  

---

## 🔌 Pin Connections

| Component         | Arduino Pin |
|-------------------|-------------|
| Servo Motor (signal) | 3         |
| Ultrasonic Trigger  | 10        |
| Ultrasonic Echo     | 11        |
| Buzzer             | 9          |
| Red LED            | 5          |
| Blue LED           | 6          |
| Green LED          | 7          |

---

## ▶️ How to Run
1. Upload the sketch (`sonar_scanner.ino`) to your Arduino board.  
2. Connect the components according to the table above.  
3. Power up the Arduino.  
4. Watch the servo sweep and observe LED + buzzer alerts as objects move closer or farther.  

---


