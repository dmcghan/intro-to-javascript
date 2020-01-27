# Module 1: JavaScript Basics

## Introduction

In this module you will start working with the basics of JavaScript including variables, operators, and functions - all from the console in your browser's developer tools. 

This module is based on [Google Chrome's DevTools](https://developers.google.com/web/tools/chrome-devtools/), so use that browser if possible. You may use a different browser if needed, but you'll need to adapt the instructions the follow as needed.

***To log issues***, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Module 1 Objectives

- Become familiar with the browser's console
- Learn how to declare variables and work with operators
- Learn how to create and execute functions

## Parts

### **Part 1:** Using the browser's console

In this part, you will learn how to declare variables and work with different operators.

1.  In Chrome, press **Command+Option+J** (Mac) or **Control+Shift+J** (Windows/Linux) to open the DevTools Console tab.

    ![](images/1/open-console.png)

2.  The developer tools window can be docked to the browser in different ways or completely undocked. Take a moment to practice resizing and changing the position of the developer tools window using the customization menu. 

    Go to the next step when you have the developer tools window positioned as you like it.

    ![](images/1/devtools-dock-side.png)

3.  Type the following code into the **Console** tab. Try typing it out, rather than copy-pasting it. Note that pressing **Enter** will execute the code in the console. Use **Shift+Enter** to add new lines. 

    ```
    var var1 = 1;
    var var2 = 2;

    var1 + var2;
    ```

4.  Press **Enter** to execute the code entered in the previous step. You should see the number `3` output to the console.

    ![](images/1/repl-output.png)

    As you can see, the console is an implementation of a Read-Eval-Print-Loop (REPL). It reads your code, executes it, prints the output from the last expression, and then returns control to you to do it all over again.

5.  Press the **Up Arrow** to load the previously executed block of code. Note that the **Up Arrow** and **Down Arrow** can be used to cycle through the console's execution history. Modify the code so that it appears as follows.

    ```
    var var1 = 1;
    var var2 = 2;

    console.log(var2 - var2);
    console.log(var1 + var2);
    ```

6.  Press **Enter** to execute the code. You should see output like the following in the console.

    ![](images/1/console-log-output.png)

    As you can see, `console.log` method provides a means of getting output from JavaScript code. This can be useful for simple debugging.

    `undefined` is shown at the end because the last statement (a call to `console.log`) did not return a value. It's as though it returned `undefined`.

7.  Return to the console and begin typing the name of one of the variables declared in the previous code (e.g. `var1`). You should see an autocomplete popup window that shows the names of both variables.

    ![](images/1/auto-complete.png)

    Note that if you type the full name of a variable and press **Enter**, the value of the variable will be displayed in the console.

8.  Refresh the web page and try typing the name of a variable again. They will not show up because the each time a page is loaded in the browser it gets its own new JavaScript context. 

### **Part 2:** Variables, data types, and operators

Now that you have a basic working knowledge of the console, it's time to get your hands dirty working with JavaScript.

Plan: 

1.  Enter the following code in the console. Use the variables as a guide to add four new variables, one of each type. Press **Enter** as use the console to see the values of the variables.

    ```
    var msg = 'Hello';
    var id = 123;
    var fun = true;
    var things = ['car', 'laptop', msg];
    ```

2.  Add on to the code from the previous step by writing statements that use the following operators. Choose at least 2 operators from each of the 4 types for a minimum of 8 statements.

    | Operator Type | Operators |
    | --- | --- |
    | Assignment | `=`, `+=`, `-=`, `*=`, `/=`, `%=` |
    | Arithmetic | `+`, `-`, `*`, `/`, `%`, `++`, `--` |
    | Comparison | `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=` |
    | Logical | `&&`, `||`, `!` |

### **Part 3:** Conditionals and loops

Programming wouldn't be possible without conditionals and loops. The basic `if` statement and `for` loop are all you really need to get going with JavaScript.

1.  Add on to the code from the previous part by writing an `if` statement of your choosing. Use the following code as a guide.

    ```
    if (msg === 'bye') {
      fun = false;
    }
    ```

    Run your code a of couple times to test it. For extra practice, write an `if-then-else` statement.

2.  Add on to the code from the previous step by writing a loop that displays the values in the array you declared in Step 1. Use the following code as a guide.

    ```
    for (var x = 0; x < things.length; x += 1) {
      console.log(things[x]);
    }
    ```

    Run your code a of couple times to test it.

### **Part 4:** Objects and functions

Objects and functions are used to organize and compose code in JavaScript. It's important to have a basic understanding of how they work before moving on to more complex topics.

1.  Enter the following code into the console and execute it.

    ```
    var person = {
      first: '',
      last: ''
    };

    function sayHello(p) {
      console.log('Hi ' + p.first + ' ' + p.last);
    }
    ```

2.  Using the console, type and execute code that sets the values of the `first` and `last` attributes of the `person` variable.

3.  Using the console, type and execute code that invokes the `sayHello` function while passing it the `person` variable.

## Summary

This completes Module 1. At this point, you should feel comfortable working with some of the core constructs of JavaScript and browser's console. [Click here](2-create-an-app-from-a-spreadsheet.md) to navigate to Module 2.