Cats mature at a faster rate than human beings. We often say a cat's age can be calculated in "cat years" to account for their growth compared to a human of the same age. In some ways we could say, time moves quickly for cats — 8 years in a human's life equates to 64 years in a cat's life. While there's no reliable scientific way to calculate the relationship between human and cat years we are going to work with a recommended formula to find out how old would you be if you were a cat.

Challenge: Convert Your Age to Cat Years

Here's how you convert your age from "human years" to "cat years":

The first two years of a cat's life count as 25 cat years each.

Each year following equates to 4 cat years.

Instead of trying to do this math in your head, let's create an application that does this for us! With your knowledge of math operators and variables, use PHP to convert your human age into cat years. If at any point you get stuck during this challenge feel free to skip ahead to the next video to see the solution I implement.

1. Begin by creating a variable named `my_age`, and set it equal to your age as a number. Write a comment that explains this line of code.

2. Next, create a variable named `early_years` and save the value `2` to it. Note, the value saved to this variable will change. Write a comment that explains this line of code.

3. Use the multiplication assignment operator `*=` to multiply the value saved to `early_years` by `25` and reassign it to `early_years`. This will account for the first two years of a cats life where they experience accelerated growth. Write a comment that explains this line of code.

4. Since we already accounted for the first two years, take the `my_age` variable, and subtract `2` from it. Set the result equal to a variable called `later_years`. We'll be changing this value later. Write a comment that explains this line of code.

5. Multiply the `later_years` variable by `4` to calculate the number of cat years accounted for by your later years. Use the multiplication assignment operator `*=` to multiply and assign in one step. Write a comment that explains this line of code.

6. If you'd like to check your work at this point, `echo`the values of `early_years` and `later_years`. Are the values what you expected?

7. Go ahead and delete the `echo`'s  from step 6. Add `early_years` and `later_years` together, and store that in a variable named `my_age_in_cat_years`.

Write a comment that explains this line of code.

8. Save the value of your name to the variable `my_name`. Write your name as a string and store the result in a variable called `my_name`. Write a comment that explains this line of code.

9. `echo` a statement that displays your name and age in cat years. Use string concatenation or string interpolation to display the value in the following sentence:
```
My name is NAME. I am HUMAN AGE years old in human years which is CAT AGE years old in cat years.
```
Replace  "NAME" with `my_name`, "HUMANE AGE" with `my_age`, and  "CAT AGE" with `my_age_in_cat_years` in the sentence above.

Write a comment that explains this line of code.

That's it! Congratulations. Here are a couple of images of cats shooting lasers out of their eyes for all your hard work :) If you got stuck or would like to see my solution please check out the next video.

Completed Code: 
```
<?php
// assign my age to the variable `myAge`
$my_age = 20;

// assign value of `2` to variable `earlyYears`
$early_years = 2;

// multiply `earlyYears` by `25` to account for early growth rate
$early_years *= 25;

// subtract `2` years from `myAge` and assign to `laterYears` to account for growth rate of a 
// cat after the first two years
$later_years = $my_age - 2;

$later_years *= 4;

// add value of `earlyYears` and `laterYears` for the total age and assign to `myAgeInCatYears`
$my_age_in_cat_years = $early_years + $later_years;

// assign the value of my name to the variable `myName`
$my_name = 'Rob';

echo 'My name is ' . $my_name . '. I am ' . $my_age 
. ' years old in human years which is ' . $my_age_in_cat_years 
. ' years old in cat years.';
```