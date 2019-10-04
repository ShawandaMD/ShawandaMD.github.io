---
layout: post
title:      "Scope and Hoisting Refresher"
date:       2019-10-04 10:56:47 -0400
permalink:  scope_and_hoisting_refresher
---


Variable declarations seem simple enough until you're wondering if the variable you created outside of your function and where you actually assigned the variable is going to return back the information you need.

As a new Javascript developer this appears to be something I need to thoroughly understand in order to get comfortable with Javascript…

So let’s get into it shall we?

#### Defining the terms.

**Scope-** is where declared functions or variables have access or is available in your code.

**Hoisting-** the action of moving all variable and function declarations to the top of the current scope.


## SCOPE

Scope is important because it allows developers to easily follow/ debug code that has been given specific visibility to a specific area of code


#### 3 TYPES OF SCOPE

#### Global
Variables and functions declared here are accessible everywhere in the code.

#### Function
Also known as local scope. Variables declared inside a function, can only be accessed from inside that function and will not be recognized or defined outside of it

#### Block
Variables declared in a block (Think curly brackets within an if statement) are not visible outside of the block.(Variables declared with var are not block scoped)

### SCOPE CHAIN

This is how Javascript determines scope!

What matters here is where the function is declared. This means the engine will first look in its current scope to see if it has access and will continue to venture outwards until it finds its match. Regardless of where the function is invoked, scope chain cares about where it is being declared. This is also known as lexical scoping. 


## HOISTING
When the engine is compiling all code from top to bottom, it is scanning for function and variable declarations and these variables live in the Lexical Environment during execution.

And depending on the order of when functions are being declared, this determines the results at run time.

In relation to where the variables are being assigned, it’s helpful to know that only actual function declarations are hoisted. Another thing to note is that `var` is also hoisted and its declaration is initialized as undefined at run time.

To avoid any bugs or issues with Hoisting it’s best to use `let` and `const` because even while hoisted these declarations remain uninitialized because the engine doesn't allow them to be referenced before they've been initialized.

If you are going to use `var`, the rule for function declaration is to declare it at the ***top*** of the scope.

The best way to get a better understanding of Scope and Hoisting is to play around with basic functions and variable declarations in your console!

Practice makes progress!

### -S
