# BasicArduino
I'm going to learn how to use an Arduino, and make awesome things with it!


## TableofContents
* [TableOfContents](#TableOfContents)
* [HelloArduino](#HelloArduino)
* [FiniteLEDBlink](#FiniteLEDBlink)

## HelloArduino

### Description & Code

```C++

  void setup() {
  Serial.begin(9600);
  Serial.println("Hello World");
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(13, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  Serial.println("Blink");
  digitalWrite(13, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(100);                       // wait for a second
  digitalWrite(13, LOW);    // turn the LED off by making the voltage LOW
  delay(100);                       // wait for a second
}
  // I went to office hours and Mr.H helped me and it definatly made me undestand the arduino and code a lot better.

```

### Evidence
[Here is my code on Arduino Create](https://create.arduino.cc/editor/jmyhre21/38142e8f-038e-4b3d-a254-b2024cdc2033)

### Image or Wiring
![Image of wiring](https://cdn.sparkfun.com/r/600-600/assets/learn_tutorials/3/1/0/sik_redboard_circuit_01.png)
### Reflection
This made me feel like I did something when I got it and it was really fun trying to figure it out.

## FiniteLEDBlink

### Description & Code

```C++
Code Goes Here
```

### Evidence

### Image or Wiring

### Reflection
