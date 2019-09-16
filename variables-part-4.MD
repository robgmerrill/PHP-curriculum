# Strings and Variables
You might be tired of using so many `""` and `.` while concatenating variables to your strings. You might be wondering if there is a better way? 

There is!

We can actually place variables directly into double quoted strings. 

Let's look at our previous attempt:
```
<?php
$villain = "Voldemort";
$hero = "Harry Potter";
$movie_title = "Chamber of Secrets";

echo $hero . " battles against " . $villain . " in the movie " . $movie_title . ".";
```

The alternative and more convenient to code solution is:
```
<?php
$villain = "Voldemort";
$hero = "Harry Potter";
$movie_title = "Chamber of Secrets";

echo "$hero battles against $villain in the movie $movie_title.";
```

That was way easier wasn't it? These variables are parsed which means the computer will read the variables as the value they hold rather than see them as just characters to be displayed.

Remember, this has to be with double quoted strings `""`. Look what happens to the output if we do single quotes:
```
<?php
$villain = "Voldemort";
$hero = "Harry Potter";
$movie_title = "Chamber of Secrets";

echo "$hero battles against $villain in the movie $movie_title.";
echo '$hero battles against $villain in the movie $movie_title.';
```

If we look at our second `echo` using single quotes the PHP outputs the variables as just text instead of their values they are referring to: `$hero battles against $villain in the movie $movie_title.`

Now that we have this new tool what could possibly go wrong?

Here is something. Let's take a look at this code: 
```
<?php
$pet = "dog";
echo "I like to pet $pets.";
```

Our hope is that we would print out the sentence: `I like to pet dogs.`

We are going to get an error: `PHP Notice:  Undefined variable: pets...`

Remember, PHP is going to look at all the characters after the `$` and look for a matching variable name. In our case we have a `$pet` variable but PHP is looking for a `$pets` variable.

So how do we workaround this problem?

Curly braces `{}` to the rescue!

We'll keep our `$` sign but the remainder of our variable name within `{}`. 

Let's revisit our above example:

```
<?php
$pet = "dog";
echo "I like to pet ${pet}s.";
```

Now, when we run our code we get the output that we would expect: `I like to pet dogs.`

PHP successfully finds our `$pet` variable and we are able to then add an `s` in the string where we wanted to get the plural `dogs`.

Want to practice further?
Go to the following link and you will find your repl prepopulated with some code: https://repl.it/@robgmerrill/variable-madlibs

Here is an exercise:
We are going to complete a madlib. A madlib is where a person chooses random verbs, nouns, adjectives...etc and then they are plugged into an already written story.

1. In the sentence there are variables named `$noun`, `$verb` and `$adjective`. Please give each empty string a noun, verb and adjective.

2. In our story replace the empty blanks `____` with a variable in the order they are listed. Run your code to make sure that your madlib prints!

3. There is a second challenge below. If you uncomment out the line `// echo "\nI have always wanted to hang out with $nouns. They are always $verbing $adjectiveish.";` you will get an error.

Fix the code and run it to make sure that you have removed your errors.

Possible Solution:
```
<?php
// Give string values to the variables below to complete the madlib:
  $noun = "shark";
  $verb = "swim";
  $adjective = "quick";


  echo "I had a dream that I was a $noun. I was being chased by a giant slug. To get away I $verb $adjective to avoid getting slimed!";


// Edit the code below to avoid errors and uncomment it:

 echo "\nI have always wanted to hang out with ${noun}s. They are always ${verb}ing ${adjective}ish.";
```