
<p align="center">
<img src="https://github.com/Niraj-Roy/stopwatch/blob/main/Dmxv.gif">
</p>
<h1>

🔗[CLICK HERE TO SEE STOPWATCH](https://stopw4tch.netlify.app/)  

</h1>
<H2> PREVIEW </H2>

<img src ="https://github.com/Niraj-Roy/stopwatch/blob/main/IMG_20220102_132846.jpg">
<h2 align="center" > Let's see how it works </h2>
        

       const timer = document.getElementById('stopwatch'); 

This Function imports the timer 'div' as a variable, using it's id, so we can modify it as we wish.


       var hr = 0; var min = 0; var sec = 0;

 we are creating the hour, minute and second variables and we are declaring that their initial value is 0.

      var stoptime = true;

 we create a variable so we can then verify if the stopwatch is running or not.

      if (stoptime == true) { stoptime = false; timerCycle(); } 

if the stopwatch is not running, turn it on and go to the timerCycle() function. (This only runs if we click the 'Start' button)

      if (stoptime == false) { stoptime = true; } 

if the stopwatch is running, turn it off. (This only runs if we click the 'Stop' button)

      if (stoptime == false) 

{ verify that the stopwatch is on.

      sec = parseInt(sec); min = parseInt(min); hr = parseInt(hr);

 these are used to parse a string into an integer. (if we have 1045 as a string and we want to use it as an integer, we parse it)
      
      sec = sec + 1; 

add 1 to seconds.

      if (sec == 60) 

if seconds are equal to 60, minutes = 1 and seconds becomes 0 again.

      if (min == 60) 

 if minutes are equal to 60, hours = 1 and seconds + minutes becomes 0 again.
