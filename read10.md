[**HOME**](https://mousasbbah.github.io/reading-notes/) 


# JavaScript : Error Handling & Debugging

## ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.


|PROPERTY |DESCRIPTION|
|--|--|
`name` |Type of executionmessage Description|
`fileNumber` |Name of the JavaScript file
`lineNumber`| Line number of error

***


There are seven types of built-in error objects in
JavaScript : 


|OBJECT|DESCRIPTION|
|---|---|
|`Error`|Generic error - the other errors are all based upon this error
`Syntax Error`|Syntax has not been followed|
|`Ref erenceError`| Tried to reference a variable that is not declared/within scope|
|`TypeError`|An unexpected data type that cannot be coerced|
|`Range Error`|Numbers not in acceptable range|
|`URI Error`|encodeURI ().decodeURI(),and similar methods used incorrectly|
|`EvalError`|eva l () function used incorrectly|


## HOW TO DEAL WITH ERRORS
* DEBUG THE SCRIPT TO FIX ERRORS

  If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.


* HANDLE ERRORS GRACEFULLY
   You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement s.

## Code Debugging
Programming code might contain syntax errors, or logical errors.

Many of these errors are difficult to diagnose.

Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

Searching for (and fixing) errors in programming code is called code debugging.

### **JavaScript Debuggers**

Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger.

Built-in debuggers can be turned on and off, forcing errors to be reported to the user.

With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing.

Normally, otherwise follow the steps at the bottom of this page, you activate debugging in your browser with the F12 key, and select "Console" in the debugger menu.

### **Setting Breakpoints**
In the debugger window, you can set breakpoints in the JavaScript code.

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.

After examining values, you can resume the execution of code (typically with a play button).

## **The debugger Keyword**
The **`debugger`** keyword stops the execution of JavaScript, and calls (if available) the debugging function.

This has the same function as setting a breakpoint in the debugger.

If no debugging is available, the debugger statement has no effect.

With the debugger turned on, this code will stop executing before it executes the third line.

[HOME](https://mousasbbah.github.io/reading-notes/) 