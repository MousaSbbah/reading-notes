[Home Page](https://mousasbbah.github.io/reading-notes)


# Functions

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 

<br>

## Function declarations
A function definition (also called a function declaration, or function statement) consists of the `function` keyword, followed by:

   * The name of the function.
   * A list of parameters to the function, enclosed in parentheses and separated by commas.
   * The JavaScript statements that define the function, enclosed in curly brackets, {...}.

For example :

`` function square(number) {
  return number * number;
}``

## Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

`` square(5); ``
