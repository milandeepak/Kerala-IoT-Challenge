---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

# <u><b>Kerala IoT Challenge</b></u>
<blockquote>
  <p><strong>Foxlab Makerspace</strong> in association with <strong>GTech - Group of Technology Companies</strong> in Kerala is launching our prestigious program  <strong>“Kerala&nbsp;IoT Challenge 2021”</strong>,  with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. <strong>Kerala IoT Challenge</strong> is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.</p>
</blockquote>

# <u><b>About Me</b></u>
<blockquote>
Hi, I am  Milan Deepak. I am a first year Electronics and Communications student  @ <a href="http://mgmits.ac.in/" target="_blank">Muthoot&nbsp; Institute&nbsp; of&nbsp; Technology&nbsp; and&nbsp; Science</a>.
I have helped in some electronics projects. I love to learn new things and I like to be updated with development in the Tech Industry. I am Fascinated  about Tech, Space and related stuff.  
</blockquote>
____

# <u><b>LEVEL - I</b></u>

# <u><b>Experiments</b></u>

## Exp 1 : Hello World LED Blinking

### Hardware Needed:
   * Arduino Uno Board x1
   * USB Cable x1
   * LED (Any Color) x1
   * 220 OHM Resistor X1 
   * Breadboard
   * Jumper Wires (Male to Male ) x2

### Code
    int ledPin = 10; // define digital pin 10.
    void setup()
    {
     pinMode(ledPin, OUTPUT);// define pin with LED connected as output.
    }
    void loop()
    {
     digitalWrite(ledPin, HIGH); // set the LED on.
     delay(1000); // wait for a second.
     digitalWrite(ledPin, LOW); // set the LED off.
     delay(1000); // wait for a second
    }


### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/EjBNj1aGhZI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

___


## Exp 2 : Traffic Light

### Hardware required
  * Arduino board x1
  * USB cable x1
  * Red M5 LED x1
  * Yellow M5 LED x1
  * Green M5 LED x1
  * 220Ω resistor x3
  * Breadboard x1
  * Breadboard jumper wires as needed

### Code
    int red =10; // initialize digital pin 8.
    int yellow =7; // initialize digital pin 7.
    int green =4; // initialize digital pin 4.
    void setup()
    {
      pinMode(red, OUTPUT);// set red LED pin as “output”
      pinMode(yellow, OUTPUT); // set yellow LED pin as  “output”
      pinMode(green, OUTPUT); // set green LED pin as “output”
    }
    void loop()
    {
      digitalWrite(green, HIGH);// turn on green LED
      delay(5000);// wait 5 seconds
      digitalWrite(green, LOW); // turn off green LED
      for(int i=0;i<3;i++)// blinks for 3 times
      {
       delay(500);// wait 0.5 second
       digitalWrite(yellow, HIGH);// turn on yellow LED
       delay(500);// wait 0.5 second
       digitalWrite(yellow, LOW);// turn off yellow LED
      } 
      delay(500);// wait 0.5 second
      digitalWrite(red, HIGH);// turn on red LED
      delay(5000);// wait 5 seconds
      digitalWrite(red, LOW);// turn off red LED
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/-Da8OEcXSas" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

___

## Exp 3 : LED Chasing Effect

### Hardware required
  * LED x6
  * Arduino board x1
  * 220Ω resistor x6
  * Breadboard x1
  * USB cable x1
  * Breadboard wire x13

### Code
    int first= 2;  // the I/O pin for the first LED
    int last= 6;   // number of LEDs
    void setup(){
     for (int i = start; i < first + last; i ++){
      pinMode(i, OUTPUT);   // set I/O pins as output
     }
    }
    void loop(){
     for (int i = BASE; i < start +; i ++){
      digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
      delay(200);        // delay
    }
     for (int i = BASE; i < BASE + NUM; i ++){
      digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
      delay(200);        // delay
     }  
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/dLirEbPWCPg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

## Exp 4 : Button Controlled LED

### Hardware required
* Arduino Uno
* Button switch*1
* Red M5 LED*1
* 220ΩResistor*1
* 10KΩ Resistor*1
* Breadboard*1
* Breadboard Jumper Wire*6
* USB cable*1

### Code
    int ledpin=11;// initialize pin 11
    int inpin=3;// initialize pin 3
    int val;// define val
    void setup()
    {
    pinMode(ledpin,OUTPUT);// set LED pin as “output”
    pinMode(inpin,INPUT);// set button pin as “input”
    }
    void loop()
    {
    val=digitalRead(inpin);// read the level value of pin 3 and assign if to val
    if(val==LOW)// check if the button is pressed, if yes, turn on the LED
    { digitalWrite(ledpin,LOW);}
    else
    { digitalWrite(ledpin,HIGH);}
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/xiQ2F2ps62I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

## Exp 5 : Buzzer

### Hardware required
* Arduino Uno
* Buzzer x1
* Breadboard x1
* Breadboard Jumper Wire x2
* USB cable x1

### Code
    int buzzer=8;// initialize digital IO pin that controls the buzzer
    void setup() 
    { 
      pinMode(buzzer,OUTPUT);// set pin mode as “output”
    } 
    void loop() 
    {
    digitalWrite(buzzer, HIGH); // produce sound
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/QN5DBPFhgCU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

## Exp 6 : RGB LED

### Hardware required
* Arduino Uno
* USB Cable x1
* RGB LED x1
* Resistor x3
* Breadboard jumper wire x5

### Code
    int redpin = 11; //select the pin for the red LED
    int bluepin =10; // select the pin for the blue LED
    int greenpin =9;// select the pin for the green LED
    int val;
    void setup() {
      pinMode(redpin, OUTPUT);
      pinMode(bluepin, OUTPUT);
      pinMode(greenpin, OUTPUT);
      Serial.begin(9600);
    }
    void loop() 
    {
    for(val=255; val>0; val--)
      {
      analogWrite(11, val);
      analogWrite(10, 255-val);
      analogWrite(9, 128-val);
      delay(1); 
      }
    for(val=0; val<255; val++)
      {
      analogWrite(11, val);
      analogWrite(10, 255-val);
      analogWrite(9, 128-val);
      delay(1); 
      }
    Serial.println(val, DEC);
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/CHlVNigktpU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

## Exp 7 : LDR Light Sensor

### Hardware required
* Arduino Uno Board
* Photo Resistorx1
* Red M5 LED x1
* 10KΩ Resistor x1
* 220Ω Resistor x1
* Breadboard x1
* Breadboard Jumper Wire x5
* USB cable x1

### Code
    void setup() {
      pinMode(8,INPUT);
      pinMode(9,OUTPUT);
      Serial.begin(9600); //initialise serial monitor
    }

    void loop() {
      int temp=digitalRead(8);       //assign value of LDR sensor to a temporary variable
      Serial.println("Intensity="); //print on serial monitor using ""
      Serial.println(temp);         //display output on serial monitor
      delay(300);
      if(temp==HIGH)               //HIGH means,light got blocked
      digitalWrite(9,HIGH);        //if light is not present,LED on
      else
      digitalWrite(9,LOW);         //if light is present,LED off
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/ae_OpAmNPWU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

## Exp 8 :Flame Sensor

### Hardware required
* Arduino Uno Board x1
* Flame Sensor x1
* Buzzer x1
* 10K Resistor x1
* Breadboard Jumper Wire x6
* USB cable x1

### Code
    int flame=0;// select analog pin 0 for the sensor
    int Beep=9;// select digital pin 9 for the buzzer
    int val=0;// initialize variable
    void setup() 
    {
      pinMode(Beep,OUTPUT);// set LED pin as “output”
      pinMode(flame,INPUT);// set buzzer pin as “input”
      Serial.begin(9600);// set baud rate at “9600”
    } 
    void loop() 
    { 
      val=analogRead(flame);// read the analog value of the sensor 
      Serial.println(val);// output and display the analog value
      if(val>=600)// when the analog value is larger than 600, the buzzer will buzz
      {  
        digitalWrite(Beep,HIGH); 
      }
      else 
      {  
        digitalWrite(Beep,LOW); 
      }
      delay(500); 
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/Rg8-zSdH2Bo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___

## Exp 9 : LM35 Temperature Sensor

### Hardware required
* Arduino Uno  Board x1
* LM35 x1
* Breadboard x1
* Breadboard Jumper Wire x5
* USB cable x1

### Code
    int potPin = 0; // initialize analog pin 0 for LM35 temperature sensor
    void setup()
    {
      Serial.begin(9600);// set baud rate at”9600”
    }
    void loop()
    {
      int val;// define variable
      int dat;// define variable
      val=analogRead(0);// read the analog value of the sensor and assign it to val
      dat=(125*val)>>8;// temperature calculation formula
      Serial.print("Tep");// output and display characters beginning with Tep
      Serial.print(dat);// output and display value of dat
      Serial.println("C");// display “C” characters
      delay(500);// wait for 0.5 second
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/dGA-OZRmgXc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___

## Exp 10 : IR Remote Control Using TSOP

### Hardware required
* Arduino Uno Board x1
* Infrared Receiver x1
* Infrared Remote Controller x1
* Breadboard x1
* LED x2
* 220ΩResistor x2
* Breadboard Jumper Wires as needed
* USB cable x1

### Code
    #include <IRremote.h>
    int RECV_PIN = 11;
    int LED1 = 2;
    int LED2 = 3;
    long on1  =0xEFB24D;
    long on2 = 0xEF728D;
    IRrecv irrecv(RECV_PIN);
    decode_results results;
    // Dumps out the decode_results structure.
    // Call this after IRrecv::decode()
    // void * to work around compiler issue
    //void dump(void *v) {
    //  decode_results *results = (decode_results *)v
    void dump(decode_results *results) {
      int count = results->rawlen;
      if (results->decode_type == UNKNOWN) 
        {
        Serial.println("Could not decode message");
        } 
      else 
      {
        if (results->decode_type == NEC) 
          {
          Serial.print("Decoded NEC: ");
          } 
        else if (results->decode_type == SONY) 
          {
          Serial.print("Decoded SONY: ");
          } 
        else if (results->decode_type == RC5) 
          {
          Serial.print("Decoded RC5: ");
          } 
        else if (results->decode_type == RC6) 
          {
          Serial.print("Decoded RC6: ");
          }
        Serial.print(results->value, HEX);
        Serial.print(" (");
        Serial.print(results->bits, DEC);
        Serial.println(" bits)");
      }
        Serial.print("Raw (");
        Serial.print(count, DEC);
        Serial.print("): ");
    for (int i = 0; i < count; i++) 
        {
          if ((i % 2) >= 1) {
          Serial.print(results->rawbuf[i]*USECPERTICK, DEC);
        } 
        else  
        {
          Serial.print(-(int)results->rawbuf[i]*USECPERTICK, DEC);
        }
        Serial.print(" ");
        }
          Serial.println("");
        }
    void setup()
    {
      pinMode(RECV_PIN, INPUT);   
      pinMode(LED1, OUTPUT);
      pinMode(LED2, OUTPUT);
      pinMode(13, OUTPUT);
      Serial.begin(9600);
      irrecv.enableIRIn(); // Start the receiver
    }
    int on =0;
    unsigned long last = millis();
    void loop() 
    {
      if (irrecv.decode(&results)) 
      {
        // If it's been at least 1/4 second since the last
        // IR received, toggle the relay
        if (millis() - last > 250) 
          {
            on =  ! on;
    //        digitalWrite(8, on ? HIGH : LOW);
            digitalWrite(13, on ? HIGH: LOW);
           dump(&results);
          }
        if (results.value == on1 ){
          digitalWrite(LED1, HIGH);
          delay(2000);
          digitalWrite(LED1,LOW);
        } 
        if (results.value == on2 ){
          digitalWrite(LED2, HIGH);
          delay(2000);
          digitalWrite(LED2,LOW);
        }
        
        last = millis();      
    irrecv.resume(); // Receive the next value
      }
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/TEvZmlac-Ak" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Issues faced
 <p> While compiling the code for this experiment, I got a "stray/302" error. When I searched it up here <a href="https://stackoverflow.com/questions/19198332/compilation-error-stray-302-in-program-etc">Link</a> , I realised that it was because of character encoding error that happens while copying the code. So after removing them, when I compiled the code, still there were still errors. So I contacted a mentor, who told me that it was the IRremote Library issue. He told me to download this <a href="https://drive.google.com/drive/folders/1y7ny_D1WQC2eSAbUPxqiXMtTvcbymJLZ?usp=sharing">IRremote Library</a> and add it in the Arduino Libraries location(Documents\Arduino\libraries) and selecting it from the include library -> add .zip library option in the Arduino IDE. 
 After this, the code compiled without any errors(though there were some warnings, which the mentor told me to ignore).
  </p>
  <p>After this, when I used an IR remote to test the circuit, the LEDs weren't lighting up. Thats when I happen to watch a video given in the course, in which it was explained that in IR remotes different buttons gave out different codes, which the IR reciever decoded. So what I did was, when I checked the Serial Monitor, while clicking the buttons, I saw that it was displaying the code of the button pressed like this : 
 <img src="https://i.ibb.co/xYtW5hj/Screenshot-2021-09-04-221334-LI.jpg" alt="COM3" >
  So i assigned this code with 0x, like: 0xEF728D to 
  the  long on1  = 0xEF728D; replacing long on1  = 0x00FF6897;
  Repeated this for the other variables. Finally the LEDs starting lighting up when buttons were pressed.
  I am glad that I faced this issue, because I got learn more about the working of a IR remote, IR reciever and the IRremote Library. 
  </p>
___

## Exp 11 : Potentiometer analog Value Reading

### Hardware required
* Arduino Uno Board x1
* 10K Potentiometer x1
* Breadboard x1
* Breadboard Jumper Wire x3
* USB cable x1

### Code
    int potpin=0;// initialize analog pin 0
    int ledpin=13;// initialize digital pin 13
    int val=0;// define val, assign initial value 0
    void setup()
    {
      pinMode(ledpin,OUTPUT);// set digital pin as “output”
      Serial.begin(9600);// set baud rate at 9600
    }
    void loop()
    {
      digitalWrite(ledpin,HIGH);// turn on the LED on pin 13
      delay(50);// wait for 0.05 second
      digitalWrite(ledpin,LOW);// turn off the LED on pin 13
      delay(50);// wait for 0.05 second
      val=analogRead(potpin);// read the analog value of analog pin 0, and assign it to val 
      Serial.println(val);// display val’s value
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/uM4BWQmw10k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___

## Exp 12 : 7 Segment Display

### Hardware required
* Arduino Uno Board x1
* 1-digit LED Segment Display x1
* 220Ω Resistor x8
* Breadboard x1
* Breadboard Jumper Wires as needed
* USB cable x1

### Code
    int a=7;// set digital pin 7 for segment a
    int b=6;// set digital pin 6 for segment b
    int c=5;// set digital pin 5 for segment c
    int d=10;// set digital pin 10 for segment d
    int e=11;// set digital pin 11 for segment e
    int f=8;// set digital pin 8 for segment f
    int g=9;// set digital pin 9 for segment g
    int dp=4;// set digital pin 4 for segment dp
    void digital_0(void) // display number 5
    {
      unsigned char j;
      digitalWrite(a,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(e,HIGH);
      digitalWrite(f,HIGH);
      digitalWrite(g,LOW);
      digitalWrite(dp,LOW);
    }
    void digital_1(void) // display number 1
    {
      unsigned char j;
      digitalWrite(c,HIGH);// set level as “high” for pin 5, turn on segment c
      digitalWrite(b,HIGH);// turn on segment b
      for(j=7;j<=11;j++)// turn off other segments
      digitalWrite(j,LOW);
      digitalWrite(dp,LOW);// turn off segment dp
    }
    void digital_2(void) // display number 2
    {
      unsigned char j;
      digitalWrite(b,HIGH);
      digitalWrite(a,HIGH);
      for(j=9;j<=11;j++)
      digitalWrite(j,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(c,LOW);
      digitalWrite(f,LOW);
    }
    void digital_3(void) // display number 3
    {
      digitalWrite(g,HIGH);
      digitalWrite(a,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(f,LOW);
      digitalWrite(e,LOW);
    }
    void digital_4(void) // display number 4
    {
      digitalWrite(c,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(f,HIGH);
      digitalWrite(g,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(a,LOW);
      digitalWrite(e,LOW);
      digitalWrite(d,LOW);
    }
    void digital_5(void) // display number 5
    {
      unsigned char j;
      digitalWrite(a,HIGH);
      digitalWrite(b, LOW);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(e, LOW);
      digitalWrite(f,HIGH);
      digitalWrite(g,HIGH);
      digitalWrite(dp,LOW);
    }
    void digital_6(void) // display number 6
    {
      unsigned char j;
      for(j=7;j<=11;j++)
      digitalWrite(j,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(b,LOW);
    }
    void digital_7(void) // display number 7
    {
      unsigned char j;
      for(j=5;j<=7;j++)
      digitalWrite(j,HIGH);
      digitalWrite(dp,LOW);
      for(j=8;j<=11;j++)
      digitalWrite(j,LOW);
    }
    void digital_8(void) // display number 8
    {
      unsigned char j;
      for(j=5;j<=11;j++)
      digitalWrite(j,HIGH);
      digitalWrite(dp,LOW);
    }
    void digital_9(void) // display number 5
    {
      unsigned char j;
      digitalWrite(a,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(e, LOW);
      digitalWrite(f,HIGH);
      digitalWrite(g,HIGH);
      digitalWrite(dp,LOW);
    }
    void setup()
    {
      int i;// set variable
      for(i=4;i<=11;i++)
      pinMode(i,OUTPUT);// set pin 4-11as “OUTPUT”
    }
    void loop()
    {
     while(1)
     {
      digital_0();// display number 0
      delay(1000);// wait for 1s
      digital_1();// display number 1
      delay(1000);// wait for 1s
      digital_2();// display number 2
      delay(1000); // wait for 1s
      digital_3();// display number 3
      delay(1000); // wait for 1s
      digital_4();// display number 4
      delay(1000); // wait for 1s
      digital_5();// display number 5
      delay(1000); // wait for 1s
      digital_6();// display number 6
      delay(1000); // wait for 1s
      digital_7();// display number 7
      delay(1000); // wait for 1s
      digital_8();// display number 8
      delay(1000); // wait for 1s
      digital_9();// display number 9
      delay(1000); // wait for 1s
     }
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/ZbsfRioPXck" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___

# <u><b>Assignments</b></u>

## Assignment-1 : Create an automatic night lamp model using LDR and LED

### Code

    void setup() 
    {
      pinMode(8,INPUT);
      pinMode(9,OUTPUT);
      pinMode(10,OUTPUT);
      pinMode(11,OUTPUT);
      pinMode(12,OUTPUT);
      Serial.begin(9600); //initialise serial monitor

    }

    void loop() 
    {
      int temp=digitalRead(8);      //assign value of LDR sensor to a temporary variable
      delay(300);
      if(temp==HIGH)//HIGH means,light got blocked
      {
        Serial.println("LED ON"); 
        for(int i=8;i<=11;i++)
          digitalWrite(i,HIGH);

      } 
      else
      {
        Serial.println("LED OFF");
        for(int i=8;i<=11;i++)
          digitalWrite(i,LOW);
    }
    }


### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/AVfnQ8r4tMM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___

## Assignment-2 : Create a Digital Dice using 7 Segment Display and Push Button

### Code
    int buttonPin = 3;
    int buttonState;
    long ran;
    int a=7;// set digital pin 7 for segment a
    int b=6;// set digital pin 6 for segment b
    int c=5;// set digital pin 5 for segment c
    int d=10;// set digital pin 10 for segment d
    int e=11;// set digital pin 11 for segment e
    int f=8;// set digital pin 8 for segment f
    int g=9;// set digital pin 9 for segment g
    int dp=4;// set digital pin 4 for segment dp
    int time = 2000;
    void digital_1(void) // display number 1
    {
      unsigned char j;
      digitalWrite(c,HIGH);// set level as “high” for pin 5, turn on segment c
      digitalWrite(b,HIGH);// turn on segment b
      for(j=7;j<=11;j++)// turn off other segments
      digitalWrite(j,LOW);
      digitalWrite(dp,LOW);// turn off segment dp
    }
    void digital_2(void) // display number 2
    {
      unsigned char j;
      digitalWrite(b,HIGH);
      digitalWrite(a,HIGH);
      for(j=9;j<=11;j++)
      digitalWrite(j,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(c,LOW);
      digitalWrite(f,LOW);
    }
    void digital_3(void) // display number 3
    {
      digitalWrite(g,HIGH);
      digitalWrite(a,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(f,LOW);
      digitalWrite(e,LOW);
    }
    void digital_4(void) // display number 4
    {
      digitalWrite(c,HIGH);
      digitalWrite(b,HIGH);
      digitalWrite(f,HIGH);
      digitalWrite(g,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(a,LOW);
      digitalWrite(e,LOW);
      digitalWrite(d,LOW);
    }
    void digital_5(void) // display number 5
    {
      unsigned char j;
      digitalWrite(a,HIGH);
      digitalWrite(b, LOW);
      digitalWrite(c,HIGH);
      digitalWrite(d,HIGH);
      digitalWrite(e, LOW);
      digitalWrite(f,HIGH);
      digitalWrite(g,HIGH);
      digitalWrite(dp,LOW);
    }
    void digital_6(void) // display number 6
    {
      unsigned char j;
      for(j=7;j<=11;j++)
      digitalWrite(j,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(dp,LOW);
      digitalWrite(b,LOW);
    }
    void setup()
    {
      int i;// set variable
      for(i=4;i<=11;i++)
      pinMode(i,OUTPUT);// set pin 4-11as “output”
      randomSeed(analogRead(0));
    }
    void loop()
    {
      buttonState = digitalRead(buttonPin);
        if (buttonState == HIGH){
          ran = random(1, 7);
          if(ran == 1){
            digital_1();// display number 1
            delay(time);// wait for 2s
            }  
          if(ran == 2){
            digital_2();// display number 2
            delay(time);// wait for 2s
            }
          if(ran == 3){
            digital_3();// display number 3
            delay(time);// wait for 2s
            }
          if(ran == 4){
            digital_4();// display number 4
            delay(time);// wait for 2s
            }  
          if(ran == 5){
            digital_5();// display number 5
            delay(time);// wait for 2s
            }  
          if(ran == 6){
            digital_6();// display number 6
            delay(time);// wait for 2s
            } 
        }
       else 
       { 
          digitalWrite(a,LOW);
          digitalWrite(b,LOW);
          digitalWrite(c,LOW);
          digitalWrite(d,LOW);
          digitalWrite(e,LOW);
          digitalWrite(f,LOW);
          digitalWrite(g,LOW);
          digitalWrite(dp,LOW);
      } 
          
    } 

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/aHDFnTuWzFo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___
___

# <u><b>LEVEL - II</b></u>

# <u><b>Experiments</b></u>

## Exp 1 : Hello World LED Program Using Blynk App

### About
 In this experiment, an [Esp 32](https://en.wikipedia.org/wiki/ESP32)  is connected to [Blynk](https://blynk.io/) IoT platform via the internet using Wifi credentials and used to light a LED connected to the G2 pin in Esp 32. 
 The aim of the experiment is to control the LED connected to the Esp 32 using a switch created in Blynk platform which can be accessed using both Blynk web platform and mobile app. 

### Hardware Needed
   * Esp 32 x1
   * USB Cable x1
   * LED (Any Color) x1
   * Jumper wires (Female to Female) x2

### Code    
    #define BLYNK_TEMPLATE_ID "TMPLdiZuBBz4"
    #define BLYNK_DEVICE_NAME "Milan Deepak"

    #define BLYNK_FIRMWARE_VERSION        "0.1.0"

    #define BLYNK_PRINT Serial
    //#define BLYNK_DEBUG

    #define APP_DEBUG

    // Uncomment your board, or configure a custom board in Settings.h
    //#define USE_WROVER_BOARD
    //#define USE_TTGO_T7
    //#define USE_ESP32C3_DEV_MODULE
    //#define USE_ESP32S2_DEV_KIT

    #include "BlynkEdgent.h"
    BLYNK_WRITE(V0){
      int pinValue = param.asInt();
      digitalWrite(15,pinValue);
      }

    void setup()
    {
      pinMode(15,OUTPUT);
      Serial.begin(115200);
      delay(100);

      BlynkEdgent.begin();
    }

    void loop() {
      BlynkEdgent.run();
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/6uoSFZrSSdc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

___

## Exp 2 : IoT Remote Light Meter using Arduino IoT Cloud

### About
In this experiment Esp 32 is connected to [Arduino IoT Cloud](https://create.arduino.cc/iot/) via the internet using Wifi credentials and used to get values from a [LDR](https://en.wikipedia.org/wiki/Photoresistor) connected to G34(one of the analog pin) in Esp 32. The aim of this experiment read the values from the LDR when the light in the room is on or off and measuring them using a Guage and plotting them in a graph.

### Hardware Needed
   * Esp 32 x1
   * USB Cable x1
   * LDR x1
   * 10K resistor x1
   * Jumper wires (Female to Female) as needed

### Code
```
#include "thingProperties.h"

void setup() {
 pinMode(34, INPUT);
 Serial.begin(9600);
 delay(1500);

  // Defined in thingProperties.h
  initProperties();

  // Connect to Arduino IoT Cloud
  ArduinoCloud.begin(ArduinoIoTPreferredConnection);

  /*
     The following function allows you to obtain more information
     related to the state of network and IoT Cloud connection and errors
     the higher number the more granular information you’ll get.
     The default is 0 (only errors).
     Maximum is 4
  */
  setDebugMessageLevel(2);
  ArduinoCloud.printDebugInfo();
}

void loop() {
  ArduinoCloud.update();
  int val=analogRead(34);
 lightsensor=val;
 Serial.println(val);
 
}
```

### Video

<iframe width="600" height="315" src="https://www.youtube.com/embed/fZAuJH29knw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
___
___

