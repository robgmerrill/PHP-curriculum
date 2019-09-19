# `round()` `floor()` and `ceil()` methods

In this lesson we will take a sneak peak at some PHP built in functions. 

In case you forgot we are using a PHP built in function during each lesson of this course so far: `echo`

Internal or built in functions are reusable bits of code that you use throughout a project. `echo` is a built in function that you can pass a value to and that value in turn is printed to the terminal. 

In an upcoming section we will look at how to build our own functions but for now let's take a look at a few functions that can be helpful with working with numbers.

## `round()`
The `round()` method simply rounds a float:
`echo round(3.4);` outputs `3`.
`echo round(3.6);` outputs `4`.

We can also specify if we want to round a number to a specific decimal by providing a second argument (an argument is just a value that we pass to a function) to the `round()` method:

`echo round(3.44, 1);` outputs `3.4`.

`echo round(3.445, 2);` outputs `3.45`.

## `floor()`
The `floor()` method will round a float down:
`echo floor(3.7);` outputs `3`.

Like the `round()` method the `floor()` method can round to a specific decimal if a second argument is passed in:
`echo floor(3.79, 1);` outputs `3.7`.

## `ceil()`
The `ceil()` method will round a float up:
`echo ceil(3.1);` outputs `4`.

Like the two above methods `ceil()` method can round to a specific decimal if a second argument is passed in:
`echo ceil(3.71, 1);` outputs `3.8`.

Alright, we now have all the tools we need to start our first mini projects!