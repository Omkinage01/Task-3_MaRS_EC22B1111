# Task-3_MaRS_EC22B1111
  Om Ajit Kinage




INTRODUCTION:-

This is a Arduino Project for Transmitter-Receiver using a RW-630 as a Transmitter    and RW-54 as a Receiver. It is to check if the message transmitted by the RW-630 is   received by RW-54 with the help of Arduino and LED.




PSEUDO CODE:-

A)*RECEIVER*:

   1)//Defining Libraries:
     RH_ASK.h & SPI.h
   2)//Declaring Variables:
     RH_ASK rf_driver, ledPin
   3)void setup()
     a)pinMode(ledPin,pin connection);
     b)//Initialize ASK object:
       rf_driver.init();
     c)Serial.begin(9600)
   4)void loop()
     a)setting buffer size to expected mssg
     b) if(message received?)
         {
           Serial.println("Received");
           Serial.println(char*(message_name));
           digitalWrite(ledPin, HIGH);
          }
      c)if(message recieved is other than expected)
      {
          digitalWrite(ledPin, LOW);
      }

B)*TRANSMITTER*:

   1)//Defining Libraries:
     RH_ASK.h & SPI.h
   2)//Declaring Variables:
     RH_ASK rf_driver, ledPin
   3)void setup()
     a)//Initialize ASK object:
       rf_driver.init();
     b)Serial.begin(9600)
   4)void loop()
     a)//declaring and initialising the message to be sent:
         const char *msg = "Hello Word";
     b) if(message sent?)
         {
           Serial.println("Sent");
          }
      }

*The Actual Codes for transmitter and receiver are provided in another branch*





PROCEDURE:

A) Learn about the modules RW-630 and RW-54, its working and connections.
B) Also go through sample codes.
C) Make connections according to the reference site you are following.
  Receiver:
![alt text](https://how2electronics.com/wp-content/uploads/2019/08/433-mhz-arduino_bb.jpg)
  Transmitter:
![alt text](https://how2electronics.com/wp-content/uploads/2019/08/433-mhz-arduino-transmitter_bb.jpg)

D) Write the code for the modules accordingly and check if it works by running it.
E) If the code is not working or the connections then refer to another reference site.



OUTPUT:

  Case 1: Tranmitter digital connection is connected:
  ![alt text](https://drive.google.com/file/d/1tAx7b4UiFuhAqWQZ-JPxn9C8knqCvtcS/view?usp=sharing)

  Case 2: Tranmitter digital connection is disconnected:
  ![alt text](https://drive.google.com/file/d/1THdyal7UojMQ-fjMdAkDn78Vub1j5a73/view?usp=sharing)





RESOURCES:
  Reference Project link: https://how2electronics.com/433mhz-rf-module-works-interfacing-arduino/#Code_Explanation
  For Arduino Code: https://www.arduino.cc/reference/en/





THINGS YOU LEARNT:
  a) Working of RW-54 and RW-630 modules as receiver and transmitter respectively.
  b) Making a project without its previous knowledge. By accessing reference google links, codes and arduino projects.
  c) On-hand experience of Arduino, breadboard and the modules.
  d) Improved my arduino code a bit.
  e) Learnt about how things actually work in real life, different than a tinkercad project and simulations and all the problems we face with an actual module.
