# Arithmetic Operators

Now that we know how to work with integers and floating point decimals we will need to learn about arithmetic operators.

Go ahead and open up a new Repl and type out the following arithmetic operators.

## Addition and Subtraction `+` and `-`

`echo 2 + 1` outputs: `3`
`echo 2 - 1` outputs: `1`

```
$cookies_in_box = 22;
$cookies_i_ate = 12;
$total_cookies_left = $cookies_in_box - $cookies_i_ate;
echo $total_cookies_left;
```
Outputs: `10`

Also, floating point numbers will return integers if the number is whole. The following code will output `10` not `10.0`:
`echo 8.8 + 1.2`

## Division and Multiplication `/` and `*`

```
$wage_per_hour = 15;
$hours_per_week = 40;
$weekly_salary = $wage_per_hour * $hours_per_week; 
echo $weekly_salary;
```

Outputs: `600`

```
$weekly_lunch_allowance = 35;
$lunches_per_week = 5;
$cost_per_meal = $weekly_lunch_allowance / $lunches_per_week;
echo $cost_per_meal;
```
Outputs: `7`

Like addition and subtraction if floating point numbers multiply or divide to a whole number they will be an integer. The following will produce `10` not `10.0`.

`echo 2.5 * 4;`

## Exponentiation `**`

The exponention operator, `**`, is used for raising a number to the power of another number.

Here is how we would square a number by raising it to the power of 2:
`echo 8 ** 2;` outputs: `64`

Here is an example of how we would cube a number by raising it to the power of 3:
`echo 2 ** 3;` outputs: `8`

## Modulo `%`
The modulo operator may be new to you. This operator returns the remainder after the left value is divided by the right value.

`echo 10 % 3;` outputs `1`

This is because `3` goes into `10` three times with a remainder of one.

Here is a little gotcha to be careful of. The modulo operator will convert its values to integers before performing this function. `6.7 % 2.7;` will actually perform the calculation `6 % 2` returning a value of `0`.


## Order of Operations


## Mathematical Assignment Operators


Challenge: Use the echo function to print results 

1. Add two numbers together to get `13`.

2. Subtract one number from another to get `6`.

3. Multiply two floating point numbers to get `20`.

4. Divide one number by another to get `5`.

5. Raise any number to the third power.

6. If a 220 cows were broken up into heards of 45 what would be the remainder of cows left without a heard?


Possible Solution
```
<?php
// #1
echo 6 + 7;

// #2
echo 13 - 7;

// #3
echo 12.5 * 1.6;

// #4
echo 20 / 4;

// #5
echo 8 ** 3;

// #6
echo 220 % 45;

```