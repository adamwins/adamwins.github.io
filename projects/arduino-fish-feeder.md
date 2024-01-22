---
layout: project
type: project
image: img/micromouse/fishbowl.gif
title: "Automated Fish Feeder"
date: 2023
published: true
labels:
  - Engineering
  - Arduino
  - C++
summary: "I am currently developing an automated fish feeder using an arduino board."
---

<div class="text-center p-4">
  <img width="250px" src="../img/micromouse/fish-feeder.png" class="img-thumbnail" >
</div>

For this project, I wanted to practice my programming and engineering skills so I decided to automate feeding my fish out of convenience. Using an arduino board, jumper wires, and a servo motor, I am able to automate the fish food being dropped into my fish tank. I am still currently developing the shell to hold the board, but I have already completed the code for the board

This is my first experience with an arduino board so I got to learn a little bit of C++, since the arduino IDE uses a derivative of C++. I have also never been exposed to electronics so it is the first time I have used jumper wires and I needed a basic understanding of how circuits work. I have yet to design the hardware for housing the board, but that would also be a first for me as I need to use some critical thinking and engineering to accomplish the goal of my arduino.

Here is some code that illustrates how the arduino is automated:

```cpp
void loop() 
{ 
  now = millis();
  endtime = now + FISHFEEDER;
  while(now < endtime) {
   myServo.write(0);
   delay(1);
   now = millis();   
  }
  
  for(pos = 0; pos < 15; pos += 1)  // goes from 0 degrees to 15 degrees 
  {                                  // in steps of 1 degree 
    myServo.write(pos);              // tell servo to go to position in variable 'pos' 
    delay(10);                       // waits 10ms for the servo to reach the position 
  } 
  for(pos = 15; pos>=1; pos-=1)     // goes from 15 degrees to 0 degrees 
  {                                
    myServo.write(pos);              // tell servo to go to position in variable 'pos' 
    delay(10);                       // waits 10ms for the servo to reach the position 
  } 
}
```
