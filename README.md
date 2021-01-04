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

### Image of Wiring
![Image of wiring](https://cdn.sparkfun.com/r/600-600/assets/learn_tutorials/3/1/0/sik_redboard_circuit_01.png)
### Reflection
This made me feel like I did something when I got it and it was really fun trying to figure it out.

## FiniteLEDBlink

### Description & Code

```C++
int ledPin = 13;
int blinkTime = 500;
bool eyesStinging=true;


void setup()
{
  pinMode(ledPin, OUTPUT);
if(eyesStinging)                         //Only blink if it's absolutely necessary
  blinkyBlinky(5, blinkTime); // 5 is number of blinks, blinkTime is the milliseconds in each state from above: int blinkTime = 500;
}

void loop()
{


  //
}

void blinkyBlinky(int repeats, int time)// If statements tell a computer what to do with certain information
{ // You do not always need an else statement and they are used to run specific code if none of the conditions are met. And you only need an else statement if "if" in some way cannot be met.
  for (int i = 0; i < repeats; i++) // they allow the code to have different types of instructions
  {// 
    digitalWrite(ledPin, HIGH);//The double equal sign means "is equal to" and the single equal sign can be roughly translated into "is."
    delay(time);//(https://www.arduino.cc/reference/en/)
    digitalWrite(ledPin, LOW);
    delay(time);
  }
}

```

### Evidence
[Link to code](https://create.arduino.cc/editor/jmyhre21/38142e8f-038e-4b3d-a254-b2024cdc2033)
### Image of Wiring
![Image of wiring](https://cdn.sparkfun.com/r/600-600/assets/learn_tutorials/3/1/0/sik_redboard_circuit_01.png)
### Reflection
I was put in a breakout room and wes and sahana were very helpful to help me figure out the code. Sahana gave me a [link](https://forum.arduino.cc/index.php?topic=273575.0) to the code, I used the second code down and it worked without problems.
## One Button One LED

### Description and code

/*
 * Button held on pin A5 turns LED attached to pin 11 on
 */

void setup(){ 
  pinMode(11, OUTPUT);  //LED pin
  pinMode(A5, INPUT_PULLUP); //pushbutton pin    
}

void loop(){
  //if the pushbutton is pressed, hold the LED on
  if (digitalRead(A5) == LOW){ 
      digitalWrite(11, HIGH);
  } 
  else {
      digitalWrite(11,LOW);   //otherwise, turn LED off
  }
}

### Evidence
[Link to code](https://create.arduino.cc/editor/jmyhre21/3c49126e-3cc5-4d81-82f1-53e9fa6752bd)
### Image of Wiring
[Image](https://arduinogetstarted.com/images/tutorial/arduino-led-button-wiring-diagram.jpg)
### Reflection
This took me a little bit to figure out because I kept on messing up the directions of resistors and LED but I got it in the end.
