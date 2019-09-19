# Reassigning Variable Values

It will be a common occurance to reassign a value to a variable. Let's take a look at how to do that longhand and shorthand with numbers in PHP.

Let's look at an example:
```
$gas_total = 11;
echo $gas_total;
$gas_used = 1;
$gas_total = $gas_total - $gas_used;
echo gas_total;
```

Outputs:
```
11
10
```

This is such a common occurance that PHP gives us some shortcuts to do this. Let's look at how we can rewrite the example above using `-=` instead of `=`.
```
$gas_total = 11;
echo $gas_total;
$gas_used = 1;
$gas_total -= $gas_used;
echo gas_total;
```

Did you notice how we were able to completely drop `$gas_total -` from our code?

By using `-=` PHP knows that we are subtracting what comes next from `$gas_total` so we don't have to explicitly type `$gas_total`.

Let's rewrite the following code with `+=`:
```
$season_wins = 24;
$wins_this_week = 4;
$season_wins = $season_wins + $wins_this_week;
// outputs 28
```

Give it a shot! See if you can rewrite the above code with `+=`. Below is how I did it:

```
$season_wins = 24;
$wins_this_week = 4;
$season_wins += $wins_this_week;
// outputs 28
```

Let's rewrite the following examples for `/` and `%`

`*`
```
$bee_population = 1000;
$bee_population = $bee_population * 2;
```

`/`
```
$bee_population = 1000;
$bee_population = $bee_population / 2;
```

Possible Solutions:
`*=`
```
$bee_population = 1000;
$bee_population *= 2;
```

`/=`
```
$bee_population = 1000;
$bee_population /= 2;
```

Alright, great job in this lesson and we'll see you in the next!