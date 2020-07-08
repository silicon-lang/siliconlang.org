---
description: Functions are the fundamental building block of any application in Silicon.
---

# Functions

You’ve already seen one of the most important functions in the language: the `main` function, which is the entry point of many programs. You’ve also seen the `fn` keyword, which allows you to declare new functions.

_Silicon_ prefers _snake case_ as the conventional style for function and variable names. In snake case, all letters are lowercase and underscores separate words.

```text
extern fn printf(format: string, ...): i32;

// Return type (i32) will be automatically detected,
// during compile time.
fn sum(a: i32, b: i32) {
    return a + b;
}

// Return type will be considered as "void"
fn main() {
    printf("%i\n", sum(1, 2));
}

```

Function definitions in _Silicon_ start with `fn` and have a set of parentheses after the function name. The curly brackets tell the compiler where the function body begins and ends.

We can call any function we’ve defined by entering its name followed by a set of parentheses. Because `sum` is defined in the program, it can be called from inside the `main` function. Note that we defined `sum` _before_ the `main` function in the source code..

