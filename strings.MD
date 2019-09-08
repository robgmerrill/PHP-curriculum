# String Data Type

If you are new to programming languages you might be wondering what a data type is?

The PHP language has different ways of handling different data types. How a value is stored and the actions that can be performed on it will vary based on data type.

Strings represent text. It can contain letters, numbers, spaces and special characters as long as they are surrounded by single `''` or double `""` quotes.

While every part of your program is text, strings are the part we intend to keep as data rather than to be interpreted as instructions to be run by the computer.

If you want to take a look at the official PHP docs on `strings` you can look here: https://www.php.net/manual/en/language.types.string.php

Let's get on with some practice. Go ahead and open this link:

Let's use the `echo` keyword to print out the phrase `Hello PHP!'.

The `echo` keyword is how you print something or display something in PHP. 

There is also one more thing you will need to do. You always end a PHP statement with a semicolon `;`. 

Go ahead and try this with both single `'` and double `"` quotes.


```
<?php
echo "Hello PHP!";
echo 'Hello PHP!';
```

Next, turn the above code into comments. You can do that by putting a `//` or `#` in front of your code and anything that trails won't be executed by the computer.

```
<?php
// echo "Hello PHP!";
# echo 'Hello PHP!';
```

In real life you won't leave code you aren't going to use in your code base. You will want to delete it. But so we can reference code as we are learning I will often times recommend that you just comment out code for now.

Let's look at what happens when you try to create a string by wrapping text in a single `'` and double `"` quote:

```
<?php
// echo "Hello PHP!";
# echo 'Hello PHP!';
echo 'Hello PHP!";
```

When you do you will get an error `PHP Parse error:...`.

Don't worry about the error message for now. It's just important to note that this doesn't work. Because our string opens with a single `'` it is actually looking for a closing `'` but it doesn't find one so it throws an error. 

To Review:
* Any characters surrounded by single or double quotes are a data type of string.
* Strings are a data type and will not be executed as a command.

