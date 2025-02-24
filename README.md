# Javascript function with missing arguments
This repo contains a simple Javascript function that demonstrates what happens when you pass fewer arguments to a function than it is defined to accept.

## Bug
The `foo` function is defined to take two arguments, `a` and `b`. However, in the second `console.log` call, only one argument is passed.  Javascript does not automatically handle missing arguments by assigning them a default value of 0, instead it uses the value 'undefined'.  This results in a `NaN` value being returned because addition of a number and undefined is not a valid operation. 

## Solution
The solution involves setting default values for the function parameters.  This way, if an argument is omitted the function will default to a valid value and won't generate `NaN`.