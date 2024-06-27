# **Anastasia Mikhailova**
---

# **Contact information:**
---

* **Location**: Kurgan, Russia
* **Phone**: +7 9828000825
* **E-mail**: stasya3010@mail.ru
* **Telegram**: @Stasya_MikhaiLova
* **GitHub**: Stasya3010
---

## **About Me:**
---

I recently completed basic training in JavaScript, but I want to delve deeper into this topic, learn frameworks and get my first job in IT. 
My strengths are independence, perseverance, self-discipline and the ability to work in a team.
---

## **My skills:**
---
* HTML
* CSS (Bootstrap, Flexbox, SCSS)
* JavaScript (ES6, DOM, JSON API, AJAX, GSAP)
* Figma
* VSCode, WebStorm
---
## **Code Examples:**
---
A countdown application created by me as part of my JavaScript course. 
(How many days/hours/minutes/seconds are left until Christmas?)
```
function christmasCountdown() {
    const christmasDate = new Date("December 25, 2022 00:00");
    const now = new Date();
    const diff = christmasDate - now;
    
    const msInSecond = 1000;
    const msInMinute = 60 * 1000; 
    const msInHour = 60 * 60 * 1000;
    const msInDay = 24 * 60 * 60 * 1000;
 
    const displayDay =  Math.floor(diff/msInDay);
    document.querySelector(".days").textContent = displayDay;
 
    const displayHour = Math.floor((diff%msInDay) / msInHour);
    document.querySelector(".hours").textContent = displayHour;
 
    const displayMinute = Math.floor((diff%msInHour) / msInMinute);
    document.querySelector(".minutes").textContent = displayMinute;
 
    const displaySecond = Math.floor((diff%msInMinute) / msInSecond);
    document.querySelector(".seconds").textContent = displaySecond;
 


    if (diff <= 0) {
        document.querySelector(".days").textContent = 0;
        document.querySelector(".hours").textContent = 0;
        document.querySelector(".minutes").textContent = 0;
        document.querySelector(".seconds").textContent = 0;
        clearInterval(timerID);
        merryChristmas();
    
       }
    
    }

let timerID = setInterval(christmasCountdown, 1000);

function merryChristmas() {
    const heading = document.querySelector('h1');
    heading.textContent = 'MERRY CHRISTMAS HO-HO-HO!!!';
    heading.classList.add('red');
}


const button = document.querySelector('#myButton');
button.addEventListener('click', function() {
    document.querySelector('#myAudio').play();

})
```
---







