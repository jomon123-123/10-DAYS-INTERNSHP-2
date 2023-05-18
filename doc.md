1.creating a circuit using tinkercad simulator tool
2.[tinkercad](https://www.tinkercad.com)
3.created a simple RGB led circuit
![alt text](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-09%2012-06-24.png)
[related circuit](https://www.tinkercad.com/things/j22qveRhQoz-cool-maimu/editel)
# Day-3
> AND GATE
![alt text](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-11%2010-30-50.png)
> arduino uno 3 blinking circuit kpr22102210/10-Days-internship/tree/main
![arduino circuit](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-11%2011-12-00.png)
# program code of arduinohttps://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-12%2010-20-53.png


```
// C++ codehttps://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-16%2009-14-36.png
//
/*
  This program blinks pin 13 of the Arduino (the
  built-in LED)
*/

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);kpr22102210/10-Days-internship/tree/main
}

void loop()
{
  // turn the LED on (HIGH is the voltage level)
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
```
**To select the code from the tinkercad simulator** [tinker the circuit](https://www.tinkercad.com/things/fJGi43uZF9o-blinking-led/editel)
![image](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-11%2011-47-29.png) 
# DAY-4 
**program code of blinking RGB led arduino circuit**


```
// the loop routine runs over and over again forever:
void loop() {
  // read the input on analog pin 0:
  int sensorValue = analogRead(A0);
  // Convert the analog reading (which goes from 0 - 1023) to a voltage (0 - 5V):
  float voltage = sensorValue * (5.0 / 1023.0);
  // print out the value you read:
  Serial.println(voltage);
}
{
  pinMode(8, OUTPUT);
  pinMode(13, OUTPUT);
  pinMode(2, OUTPUT);
}

void loop()
{
  digitalWrite(13, HIGH);
  delay(800); // Wait for 800 millisecond(s)
   digitalWrite(13, LOW);
  delay(800); // Wait for 800 millisecond(s)
  digitalWrite(8, HIGH);
  delay(800); // Wait for 800 millisecond(s)
  digitalWrite(8, LOW);
  delay(800); // Wait for 800 millisecond(s)
  digitalWrite(2, HIGH);
  delay(800); // Wait for 800 millisecond(s)
   digitalWrite(2, LOW);
  delay(800); // Wait for 800 millisecond(s)
}
```
**To select the code from the tinkercad simulator**![image]()
[tinker the circuit](https://www.tinkercad.com/things/01X11hP2g8n-grand-hillar)
# DAY 5
**program code of potentiometer arduino circuit**



 /*
  ReadAnalogVoltage
  Reads an analog input on pin 0, converts it to voltage, and prints the result to the serial monitor.

  OPEN THE SERIAL MONITOR TO VIEW THE OUTPUT >> 
  Attach the center pin of a potentiometer to pin A0, and the outside pins to +5V and ground.

  This example code is in the public domain.
*/


// the setup routine runs once when you press reset:
void setup() {
  // initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
}

// the loop routine runs over and over again forever:
void loop() {
  // read the input on analog pin 0:
  int sensorValue = analogRead(A0);
  // Convert the analog reading (which goes from 0 - 1023) to a voltage (0 - 5V):
  float voltage = sensorValue * (5.0 / 1023.0);
  // print out the value you read:
  Serial.println(voltage);
}

![image](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-15%2014-42-02.png)
[tinker the circuit](https://www.tinkercad.com/things/6kdrijYkWY9-shiny-snicket-kieran/editel)
# DAY 6
**program code of 7 segment arduino circuit**
unsigned const int A = 13;
unsigned const int B = 12;
unsigned const int C = 11;
unsigned const int D = 10;
unsigned const int E = 9;
unsigned const int F = 8;
unsigned const int G = 7;
unsigned const int H = 6;


void setup(void)
{
  pinMode(A, OUTPUT);
  pinMode(B, OUTPUT);
  pinMode(C, OUTPUT);
  pinMode(D, OUTPUT);
  pinMode(E, OUTPUT);
  pinMode(F, OUTPUT);
  pinMode(G, OUTPUT);
  pinMode(H, OUTPUT);
}

//My Functions

void zero(void) {
  digitalWrite(A, LOW);
  digitalWrite(B, HIGH);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, HIGH);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void one(void) {
  digitalWrite(A, LOW);
  digitalWrite(B, LOW);
  digitalWrite(C, LOW);
  digitalWrite(D, HIGH);
  digitalWrite(E, LOW);
  digitalWrite(F, LOW);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void two(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, LOW);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, HIGH);
  digitalWrite(F, HIGH);
  digitalWrite(G, LOW);
  digitalWrite(H, LOW);
}

void three(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, LOW);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, LOW);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void four(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, HIGH);
  digitalWrite(C, LOW);
  digitalWrite(D, HIGH);
  digitalWrite(E, LOW);
  digitalWrite(F, LOW);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void five(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, HIGH);
  digitalWrite(C, HIGH);
  digitalWrite(D, LOW);
  digitalWrite(E, LOW);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void six(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, HIGH);
  digitalWrite(C, HIGH);
  digitalWrite(D, LOW);
  digitalWrite(E, HIGH);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void seven(void) {
  digitalWrite(A, LOW);
  digitalWrite(B, LOW);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, LOW);
  digitalWrite(F, LOW);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void eight(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, HIGH);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, HIGH);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

void nine(void) {
  digitalWrite(A, HIGH);
  digitalWrite(B, HIGH);
  digitalWrite(C, HIGH);
  digitalWrite(D, HIGH);
  digitalWrite(E, LOW);
  digitalWrite(F, HIGH);
  digitalWrite(G, HIGH);
  digitalWrite(H, LOW);
}

// Start
void loop(void)
{
  zero();
  delay(1000);
  
  one();
  delay(1000);
  
  two();
  delay(1000);
  
  three();
  delay(1000);
  
  four();
  delay(1000);
  
  five();
  delay(1000);
  
  six();
  delay(1000);
  
  seven();
  delay(1000);
  
  eight();
  delay(1000);
  
  nine();
  delay(1000);
}
![image](https://github.com/jomon123-123/10-days-internship/blob/main/Screenshot%20from%202023-05-16%2009-14-36.png)
[tinker the circuit](https://www.tinkercad.com/things/0ADi4MNSwgB-copy-of-arduino-7-segment-display/editel?tenant=circuits)
# DAY 7
> Introduced the yaskawa arm robot
1. The introduction of yaskawa AR1440 
![image](https://github.com/jomon123-123/10-days-internship/blob/main/images.jpeg)
