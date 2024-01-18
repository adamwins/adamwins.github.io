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
  <img width="200px" src="../img/micromouse/fish-feeder.png" class="img-thumbnail" >
  <video width="200px" src="../img/micromouse/IMG_4867.mov" class="img-thumbnail" >
  </video>
</div>

For this project, I wanted to practice my programming and engineering skills so I decided to automate feeding my fish out of convenience. Using an arduino board, jumper wires, and a servo motor, I am able to automate the fish food being dropped into my fish tank. I am still currently developing the shell to hold the board, but I have already completed the code for the board

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
  
  for(pos = 0; pos < 30; pos += 1)  // goes from 0 degrees to 15 degrees 
  {                                  // in steps of 1 degree 
    myServo.write(pos);              // tell servo to go to position in variable 'pos' 
    delay(10);                       // waits 10ms for the servo to reach the position 
  } 
  for(pos = 30; pos>=1; pos-=1)     // goes from 15 degrees to 0 degrees 
  {                                
    myServo.write(pos);              // tell servo to go to position in variable 'pos' 
    delay(10);                       // waits 10ms for the servo to reach the position 
  } 
}
```
