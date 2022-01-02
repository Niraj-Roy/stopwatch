# This is my First JavaScript Project :)
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


       
       var hr = 0;
       
       var min = 0; 
       
       var sec = 0;

 we are creating the hour, minute and second variables and we are declaring that their initial value is 0.

      var stoptime = true;

 we create a variable so we can then verify if the stopwatch is running or not.

      if (stoptime == true) { stoptime = false; timerCycle(); } 

if the stopwatch is not running, turn it on and go to the timerCycle() function. (This only runs if we click the 'Start' button)

      if (stoptime == false) { stoptime = true; } 

if the stopwatch is running, turn it off. (This only runs if we click the 'Stop' button)

      if (stoptime == false) {

 verify that the stopwatch is on.

      sec = parseInt(sec); 

      min = parseInt(min); 
   
      hr = parseInt(hr);

 these are used to parse a string into an integer. (if we have 1045 as a string and we want to use it as an integer, we parse it)
      
      sec = sec + 1; 

add 1 to seconds.

      if (sec == 60) {

if seconds are equal to 60, minutes = 1 and seconds becomes 0 again.

      if (min == 60) {

 if minutes are equal to 60, hours = 1 and seconds + minutes becomes 0 again.

   ```if (sec < 10 || sec == 0) {
   sec = '0' + sec;
}
if (min < 10 || min == 0) {
   min = '0' + min;
}
if (hr < 10 || hr == 0) {
   hr = '0' + hr;
}
```
If seconds, minutes and/or hours are lower than 10, add a 0 in front. This is why we need to parse everything in the beginning: doing this operation they become strings.

      timer.innerHTML = hr + ':' + min + ':' + sec;

 add these values to the 'timer' div.

     setTimeout("timerCycle()", 1000); 

this will make sure there is a timeout of 1000 ms (1s) before repeating the 'timerCycle()'.

     timer.innerHTML = '00:00:00'; 

used to reset the timer to 00:00:00


<h2 align="center">That's All , Hope u enjoyed Learning something new </h2>
