---
layout: post
title: "Math and strings in JavaScript (course note 1)"
date: 2025-04-21
categories: cybersecurity blogging
---

# Math and strings in JavaScript (course note 1)

There is an order of operations

() First

multiply and divide second (Note: These have equal priority, evaluated left-to-right)

last + and - (Note: These also have equal priority, evaluated left-to-right)

and also there is this floats problem which is common to most languages

so make sure when calculating numbers which gives answers in floats like dollars try to write it in integers (like cents) and later convert it back for display.

also if there is a calculation like ((2+2) * 55). the inner brackets are **added** first _(resulting in (4 * 55))_.

## how to round a number ?

JavaScript

```
Math.round(any_number)
```

This will round a number to the nearest integer

## strings

Strings can also be added for example 'hello'+'world' will result in helloworld

This is called concatenation

JavaScript

```
typeof 5
    // will result in number
typeof 'hello'
    // will result in string
```

This can be used to find which type of data it is

if we add a string and a number js **will** convert that number into a string and add them together

string also follow the order of operations as numbers (Note: Specifically, concatenation proceeds left-to-right)

for example if we add '$' + 500 + 500 the answer will be 500500∗(because′' + 500 happens first)*

To avoid this we can simply use '$' + (500 + 500) brackets

To make strings you can use both single and double quotes but if a single quote is already a part of the string it may interfere with the code so in that case it is best to use double quotes

But single quotes are simple and easy to read

But we can also use backtick to write strings in js

### Escape characters

but another solution to this can be to use a escape character like `\'`

for example :

JavaScript

```
'i'm a halo player'
```

this wont work because the string is ending then there is a single quote in the

One solution can be :

JavaScript

```
"i'm a halo player"
```

Another solution can be :

JavaScript

```
'i\'m a halo player'
```

using `\'` will make the single **quote** just a character in a string

### Line breaking escape characters

To break a line for example :

JavaScript

```
alert('some\ntext');
```

this will cause an input like

```
some
text
```

This is because the \n escape character