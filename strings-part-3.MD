# String Concatenation
String concatenation is when we add strings together. If you are new to programming that might sound a little strange but it is very necessary so it is an important skill to learn!

Along with learning the term "concatenation" we also are going to look at another term, `operator`. `Operator` is a character that performs some sort of task in our code. We have seen this already with the assignment operator `=` in previous lessons when assigning a string such as `"Hello PHP` to a variable `$message`.

 The `.` is the "concatenation operator". 

This will take a string on the left and combine it with the string on the right.

Go ahead and open up a new Repl:
```
<?php
echo "One string" . "Two string.";
```

Notice the output is: `One String.TwoString.` 

PHP isn't going to try to read our minds and assume that we want a space between our two sentences. We have to add that space ourself. 

We can do that at the end of the first string:
```
<?php
echo "One string " . "Two string.";
```

Or, at the beginning of the second string:
```
<?php
echo "One string" . " Two string.";
```

The results of either approach will be what we were hoping for: `One string. Two string.`

There is also another way. We could add a string that contains an empty space:

```
<?php
echo "One string" . " " . "Two string.";
```
 
Looking for some more practice with string concatenation? If so, here is a challenge: 

1. Use `echo` to print the strings `"su"`, `"per"`, `"ca"`, `"li"`, `"fra"`, `"gil"`, `"is"`, `"tic"`, `"ex"`, `"pi"`, `"a"`, `"li"`, `"do"`, `"cious"`. Don't forget the semicolon at the end!

https://www.google.com/search?q=supercalifragilisticexpialidocious+gif&sxsrf=ACYBGNQ7zUoJFjdEJmPmYewvFqwQS9T8Gw:1568041266889&tbm=isch&source=iu&ictx=1&fir=BO-LvaiF4b7HaM%253A%252ClnGfFEafHc9TNM%252C_&vet=1&usg=AI4_-kQFpxr4liHBoHb1R2yCHmkUe9pCvg&sa=X&ved=2ahUKEwiR29L1gMTkAhULTKwKHcpXBWcQ9QEwAHoECAUQBA#imgrc=BO-LvaiF4b7HaM:

Image result for supercalifragilisticexpialidocious gif

Code Solution
```
<?php
echo "su" . "per" . "ca" . "li" .  "fra" . "gil" . "is" . "tic" . "ex" . "pi" . "a" . "li" . "do" . "cious";
```