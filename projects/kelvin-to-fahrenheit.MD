In this mini-project we are going to create a mini application in the console that converts the temperature from kelvin to fahrenheit. If you don't understand the difference between fahrenheit and kelvin that is ok. I'll share with you the formula as we walk through the steps.

I will list out the 6 steps below that you need to take to build out this mini-application. In the following video I will walk through all 6 steps myself so you can see a possible solution. 

You can build out this application in any coding environment of your choice. If you are brand new to coding you may want to skip to the next video and watch the first couple minutes to see the coding environment I set up and would suggest you use. 

I will create snippets using the sources tab in the Chrome Dev Tools (The user interface of Chrom Dev Tools changes from over time. Please reach out in the Q & A if you feel these pictures don't reflect the current user experience):

Because this is our first mini-challenge you also may just want to watch me solve this challenge from start to finish to see how we solve these mini challenges then try the next mini challenge on your own.

Challenge: Convert any given temperature in Kelvin to Fahrenheit

1. Let's imagine that the weather reports says that the temperature today will be  301 Kelvin. How should you dress for the day? Let's create an app that lets us know the temperature in fahrenheit. To start, create a variable named `$kelvin_temp`, and set it equal to `301`. Write a comment above that explains this line of code.

2. Finding the temperature in Celsius is similar to Kelvin — the only difference is that Celsius is 273.15 degrees less than Kelvin.

Let's convert Kelvin to Celsius by subtracting `273.15` from the `$kelvin_temp` variable. Store the result in another variable, named `$celsius_temp`.

Write a comment above that explains this line of code.

3. Use this equation to calculate Fahrenheit, then store the answer in a variable named `$fahrenheit_temp`.

<b><i>Fahrenheit = Celsius * (9/5) + 32</i></b>

In the next step we will round the number saved to fahrenheitTemp. Write a comment above that explains this line of code.

4. Log to the console the value of  `$fahrenheit_temp`. In our next step we are going to see what we can do to make sure that our number is a whole number by rounding down. `echo`  the value to the terminal. It should begin with `82.13`.

5. As we have just seen, when you convert from Celsius to Fahrenheit, you often get a decimal number. Go ahead and delete the `echo` code from step 4.

Use the `floor()` method to round down the Fahrenheit temperature. Save the result to the `$fahrenheit_temp` variable.  Write a comment above that explains this line of code.

6. Use `echo` and string concatenation to display the temperature in `$fahrenheit_temp` to the terminal to create the message as follows:
```
The temperature is TEMPERATURE degrees Fahrenheit.
```
 TEMPERATURE should be determined by the value of `$fahrenheit_temp`.

Great job! I'll walk through these steps in the next video!

Finished Code:
```
<?php
// Temperature in kelvin stored in variable `$kelvin_temp`
$kelvin_temp = 301;

// temperature in celsius stored in variable `$celsius_temp`
$celsius_temp = $kelvin_temp - 273.15;

// convert celsius to fahrenheit stored in variable `$fahrenheit_temp`
$fahrenheit_temp = $celsius_temp * (9/5) + 32;

// round the value of fahrenheit down and assign to `$fahrenheit_temp`
$fahrenheit_temp = floor($fahrenheit_temp);

// use string concatenation to leave a message
// "The temperature is `fahrenheit` degrees Fahrenheit."
echo 'The temperature is ' . $fahrenheit_temp . ' degrees Fahrenheit.';
```