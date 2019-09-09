# Strings Part 2
So far we have learned how to create a string with opening or closing single or double quotes. 

However, what happens when our string includes quotes?

For instance, if we wanted to display the text `"Mary said, "PHP is my favorite programming language.""

Go ahead and open up a new repl and try this out.

```
<?php
echo "Mary said, "PHP is my favorite programming language."";
```

We get an error. `PHP Parse error:  syntax error, unexpected 'PHP'...`

PHP sees the opening of a string and the closing of string `"Mary said, "` then it follows with text `PHP...` that isn't surrounded by opening or closing quotes.

There are two ways that we can fix this. Instead of surrounding our text with `"` we could surround it with '`.
```
<?php
echo 'Mary said, "PHP is my favorite programming language."';
```

This works because PHP sees the opening single quote and interprets everthing as text until the closing `'`.

This is a great solution! However, we will run into situations in future lessons where this won't be an adequate solution. We don't have to worry about that for now but let's look at another way we can solve the initial problem.

## Escape Sequence `\`
Let's look at our broken code again: 
```
<?php
echo "Mary said, "PHP is my favorite programming language."";
```

We want some way to tell PHP that we don't want to treat `"Mary said, "` as the start and end of a string. We want to escape running the second `"` as the end of a string. 

An escape sequence usually consists of a backslash `\` followed by another character.

To see what this looks like in action go ahead and change our code to the following: 
```
<?php
echo "Mary said, \"PHP is my favorite programming language.\"";
```

Your code should run without any errors now. The `\` character keeps PHP from interpreting the double quotes in our sentence from being executed as code to close or open a string.

Pretty handy right?

Let's practice a little bit more. Go ahead and fix these two lines of code using the `\` approach or fix by swapping out the `'` with `"` or visa versa.

```
?php
echo "Uncle Ben said, "With great power comes great responsibility."";
echo 'I'm in.';
```

How'd it go? Your fix should look like the following:
```
<?php
echo "Uncle Ben said, \"With great power comes great responsibility.\"";
echo 'I\'m in.';
```

```
<?php
echo 'Uncle Ben said, "With great power comes great responsibility."';
echo "I\'m in.";
```

However, did you notice your output?
`Uncle Ben said, "With great power comes great responsibility."I'm in.`

It is all in one line. Even though you are on two lines of code. Also, there isn't even a space between the first and second sentence. This is hard to read and not ideal.

## Newline Escape Sequence `\n\`
The newline escape sequence `\n` can help us with this. We can put this at the end of the first string or the beginning of our second string:

End of First String:
```
<?php
echo 'Uncle Ben said, "With great power comes great responsibility."\n';
echo "I\'m in.";
```

Beginning of Second String:
```
<?php
echo 'Uncle Ben said, "With great power comes great responsibility."';
echo "\nI\'m in.";
```

Want to learn more about escape sequences? Check out the docs if you want to take a deeper dive: http://php.net/manual/en/language.types.string.php#language.types.string.syntax.double

Do you want some more practice? If so, go ahead and open up a new PHP sandbox:

Let's make an exercise accomplishment list. It is the opposite of a todo list. Instead of listing all the things you need todo you will instead list all the things that you did!

1.
Let’s make an exercise accomplishment list for you. Use `echo` to print a string to the console in the following format: 1. [thing you have done]. For example, here’s ours: 1. Run 5 miles.

2.
Let’s create a new echo statement for the next item on our exercise accomplishment list.

By default, this second statement would print on the same line as the first… Start this second string with the escape sequence for a new line character. Next, continue the string in the same format as before: 2. [Another exercise accomplishment].

3.
Let’s throw a third thing on the list. This time, let’s mix it up. Include something inside your string wrapped in double quotes. For example, here’s ours 3. Running a half marathon was a "blast".

How'd it go? Here is what a possible solution might look like:
```
<?php
echo "I did 50 burpees on Monday."
echo "\nI ran 5 miles on Tuesday."
echo "\nI ran a half marathon on Saturday. It was a \"blast\"";





