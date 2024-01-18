---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
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
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

For this project, I wanted to practice my programming and engineering skills so I decided to automate feeding my fish out of convenience. Using an arduino board, jumper wires, and a servo motor, I am able to automate the fish food being dropped into my fish tank. I am still currently developing the shell to hold the board, but I have already completed the code for the board

Here is some code that illustrates how the arduino is automated:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
