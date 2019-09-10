# Variables in Action
Once a variable has been declared and initialized it is ready to be used!

Go ahead and open up a new PHP coding sandbox and let's write the following code:

```
<?php
$villain = "Voldemort";
echo $villain;
```

`echo $villain` will output `Voldemort`.

Asside from during assignment, whenever the computer sees a variable in your code it will replace the variable with the value assignedto the variable.

This means that we can do operations on variables just as we would with any value of that type.

```
<?php
$villain = "Voldemort";
echo "The villain in Harry Potter is " . $villain . ".";
```

Output: `The villain in Harry Potter is Voldemort.`

In the above code, we concatenated the string `"The villain in Harry Potter is "` to the value held by the `$villain` variable.

Let's make some further changes to our code to get some more practice in:
```
<?php
$villain = "Voldemort";
$hero = "Harry Potter";
$movie_title = "Chamber of Secrets";

echo $hero . " battles against " . $villain . " in the movie " . $movie_title . ".";
```

This will output: `Harry Potter battles against Voldemort in the movie Chamber of Secrets.`

## Ready for a challenge?
Open up a new PHP sandbox and achieve the following steps:

1. Create variables `$name` and `$favorite_movie` and assign string values of your choice.

2. `echo` and string concatenated to the variable `$name`. End string with `\n` newline character.

3. `echo` another string concatenated with the `$favorite_movie` variable.

## Possible Solution
```
<?php
$name = "Rob Merrill";

$favorite_movie = "Hot Rod";

echo "Hi, I'm " . $name;

echo "My favorite movie that not many people know about is " . $favorite_movie . ".";
```