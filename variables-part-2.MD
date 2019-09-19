# Variable Naming Rules and Best Practices

In the last lesson we covered declaring variables and assigning values to them. 

Example of declaring a variable: 
`$name;`

Example of assigning a value: 
`$name = "Rob Merrill";`

Example of declaring and assigning at same time: 
`$weather_today = "rainy";`

In the above example we declared a variable and assigned a value in one step!

Let's talk about variables naming rules:

* All variables in PHP must start with a  `$` sign. This character allows our computer to quickly see that we are declaring a variable with our code.

* A variable name must start with a letter or the underscore character `_`. 

* A variable name cannot start with a number.

* A variable name can only contain alpha-numeric characters and underscores (`a-z`, `A-Z`, `0-9`, `_`).
 
* A variable name cannot contain spaces.

* A variable name is case sensitive. `$instructor` is different than `$iNstructor`.


## Ready for some practice?
Open up the following link and fix the following invalid PHP variables. 

Uncomment out each line of code and fix one line at a time.

Currently, if you try to `echo` the value of any of these variables you will get an error:

```
<?php
greeting = "Hello!";

$1answer = "The answer is blue.";

$favorite drink = "coffee";

$city&state = "Seattle, WA";

```

## Possible solutions
There are a lot of ways that you could have chosen to fix these variables names. 
```
<?php
# greeting = "Hello!";
# must start with a `$`
$greeting = "Hello!";

# $1answer = "The answer is blue.";
# variables names can't start with a number
$one_answer = "The answer is blue.";

# $favorite drink = "coffee";
# variables cannot contain spaces
$favorite_drink = "coffee";

# $city&state = "Seatte, WA";
# variable name can only contain alpha-numeric characters and underscores
$city_and_state = "Seattle, WA"; 
```


