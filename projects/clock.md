---
layout: project
type: project
image: img/cotton/clock.gif
title: "Clock Project"
date: 2019
published: true
labels:
  - CSS
  - HTML
  - JavaScript
summary: "A simple clock I developed using HTML, CSS, and JavaScript"
---

Back in high school, in order to practice my CSS, HTML, and Javascript, I developed a clock that updates in real time with the press of a button. Through this project, I was able to learn about JavaScript functions, as well as the basics of JavaScript since most of the clock functionality is dependent on the JavaScript code. At the time, all of this was very new to me so although it is not much now, it was a huge step forward for me in my software engineering journey. I had no prior exposure to any sort of coding so this project help set the foundation for my future of programming.

Here is some code that showcases the functionality of the clock: 
```cpp
if(h == 0){
        h = 12;
    }
    
    if(h > 12){
        h = h - 12;
        session = "PM";
    }
    h = (h < 10) ? "0" + h : h;
    m = (m < 10) ? "0" + m : m;
    s = (s < 10) ? "0" + s : s;

 var time = h + ":" + m + ":" + s + " " + session;

  var clockText = document.getElementById("MyClockDisplay").innerText = time;
  var clockContent = document.getElementById("MyClockDisplay").textContent = time;
    
}
showTime();

function refreshTime(){
  window.location.reload()
};
```
Source: <a href="https://github.com/adamanapua/clock-project"><i class="large github icon "></i>https://github.com/adamanapua/clock-project</a>
