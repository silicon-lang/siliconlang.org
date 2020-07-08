---
description: Functions are the fundamental building block of any application in Silicon.
---

# Functions

You’ve already seen one of the most important functions in the language: the `main` function, which is the entry point of many programs. You’ve also seen the `fn` keyword, which allows you to declare new functions.

_Silicon_ prefers _snake case_ as the conventional style for function and variable names. In snake case, all letters are lowercase and underscores separate words.

{% code title="src/main.si" %}
```text
extern fn printf(format: string, ...): i32;

fn hello_world() {
    printf("%s\n", "Hello World!");
}

fn main() {
    printf("%s\n", "Calling hello_world function...");
    
    hello_world();
}

```
{% endcode %}

Function definitions in _Silicon_ start with `fn` and have a set of parentheses after the function name. The curly brackets tell the compiler where the function body begins and ends.

We can call any function we’ve defined by entering its name followed by a set of parentheses. Because `hello_world` is defined in the program, it can be called from inside the `main` function. Note that we defined `hello_world` _before_ the `main` function in the source code.

#### Function Parameters

Functions can also be defined to have _parameters_, which are special variables that are part of a function’s signature. When a function has parameters, you can provide it with concrete values for those parameters. Technically, the concrete values are called _arguments_, but in casual conversation, people tend to use the words _parameter_ and _argument_ interchangeably for either the variables in a function’s definition or the concrete values passed in when you call a function.

