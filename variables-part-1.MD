# Variables
Variables are a way of referencing a value by name. 

Remember the string `"supercalifragilisticexpialidocious"`? Imagine that we wanted to use this with string concatenation a few times. 

`"The longest word I can think of is " . "supercalifragilisticexpialidocious" . "."`


`"My least favorite word to type is " . "supercalifragilisticexpialidocious" . "."`

`"The most famous word in the movie Mary Poppins is " . "supercalifragilisticexpialidocious" . "."`

That is a lot of typing the same characters over and over again? This is where variables come to the rescue!

Variables store values so we can reuse them easily through our program.

Let's look at a couple vocabulary terms we need to learn: `declare` and `assign`.

The act of `declaring` a variable is reserving the word, the variable name, which we can refer to in our code. Variable names should be human readable. There should be some hint as to what value the varialbe holds. 

In attempting to create a variable for our very long word we might choose: 
`$longest_word`

The act of `assignment` is the process of associating a variable name with a specific value so that whenever the name is referenced the computer will be able to use the value assigned to it. 

`$longest_word = supercalifragilisticexpialidocious;`

That's it! We have declared the variable `$longest_word` and assigned it a value of `"supercalifragilisticexpialidocious"`. Now, let's rewrite our earlier examples with our new variable.

`"The longest word I can think of is " . $longest_word . "."`


`"My least favorite word to type is " . $longest_word . "."`

`"The most famous word in the movie Mary Poppins is " . $longest_word . "."`

This makes a huge difference! It's a time saver and will become absolutely necessary in the future as we build out programs with PHP. 

Now, let's go ahead and take a look at a few rules and best practices for making variables.