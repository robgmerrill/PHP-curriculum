Great job making it this far!

So far we have learned: 
* who this course is for
* the format of this course
* our development environment

Let's now print "Hello PHP"!

Let's head to this link: https://repl.it/@robgmerrill/Hello-PHP

When you do you will see prepopulated content in the text editor. Each line begins with either forward slashes `//` or a `#`. 

Any code that follows `//` or a `#` is a comment. A comment is just text that we don't want our PHP interpreter to do anything with. 

It isn't for the computer. It is for YOU! It is also for those who are reading or working on your code with you. 

While we will always try to make our code easy to understand for humans sometimes as your codebase grows you may have a reason for writing some code that isn't clear days, weeks or months later when you or someone else is working on that code to add features or fix a bug. 

Comments help a human to quickly understand the code in a program. 

As you can see these comments are full of text such as `# create a variable called `$message` and give it a value of a string `"Hello PHP"``

You might be wandering what the <code>``</code> mean that are surrounding $message and "Hello PHP" in the comment?

They have a bigger purpose when not in comments but when I use them within a comment they are meant to communicate actual code I want you to write. 

So under this comment I want you to literally write `$message` and give it a value of the string `"Hello PHP"`.

Make sense? If not, that's ok, we'll work this out together. 

So under the first comment let's write out <code>$message = "Hello PHP";</code>

Perfect. That <code>=</code> is an assignment operator. Don't worry about memorizing key words such as `operator` for now. While it is good to take not of words that you may not be familiar with we will be using them over and over again to give time for them to sink in. <code>$message</code> is a variable and <code>"Hello PHP"</code> is a string. 

You will also notice the use of the semi-colon `;`. All statements in PHP have to end in a semi-colon. Don't worry too much about what the word statement means at this point. And if you ever forget PHP will give you an error message to let you know that this is missing :) 

Again, we will explain these terms in depth in a few lessons so dont' worry if that just sounds like technical jargon right now. 

Let's look at our next comment:
<code># use the `print` function to print the value of `$message`</code>

Let's try this together:
<code>print $message;</code>

Great! We just used a PHP function!

You probably didn't know it but `print` is a built in PHP function that we can pass a value to, such as <code>$message</code>, and it prints or outputs the value as you should should see on the right hand side of the screen. 

Go ahead and press the run button and you should get an output of `"Hello PHP"`. 

We'll talk about functions in depth in the future. We will look at the built in ones that are available like `print` and functions that we can create on our own :) 


Code solution:
```
# create a variable called `$message` and give it a value of a string `"Hello PHP"`
$message = "Hello PHP";

# use the `echo` function to print the value of `$message`
echo $message;
```