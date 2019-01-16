# Code Challenge: Digital Root

## What is a Digital Root?

The digital root (also repeated digital sum) of a non-negative integer is the (single digit) value obtained by an iterative process of summing digits, on each iteration using the result from the previous iteration to compute a digit sum. The process continues until a single-digit number is reached.

For example, the digital root of:

```
17 => 8 # (because 1 + 7 = 8 and 8 is a single digit number)
```

```
182 => 2 # (because 1 + 8 + 2 = 11, 11 is NOT a single digit number, so we add 1 + 1 = 2. 2 IS a single digit so we're done!)
```
Let's take a closer look at the 182 example. 

Its also true that:

```
18 + 2 = 20
2 + 0 = 2
```

So it doesn't matter if you add up each single constituent digit until you get a sum that is less than 10 (i.e. a single digit) OR if you had the last digit to the remaining number (i.e. 2 + 18) until you get to a single digit number. Either approach works.

## The Challenge
Write a method that takes in an argument of a number and returns the digital root of that number.
