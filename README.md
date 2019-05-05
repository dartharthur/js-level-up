# JavaScript Level Up

The purpose of this document is to serve as a resource for anyone who wants to level up their JavaScript and
Web Development chops.

The topics I've selected here are specifically designed to take you from a JS beginner to someone
who has a much deeper and more nuanced understanding of the language.

Therefore, this document will be most useful
for people who already have basic knowledge of JavaScript. In other words, you know what functions
and variables are, you know how to string them together to perform basic calculations, you may have heard of classes,
you've heard of `map`, `reduce`, and `filter` but don't quite understand how to use them, you know JavaScript is really
fast at I/O (input/output) but you don't know why, your understanding of the `this` keyword could be improved, etc.

Since there's already a vast amount of amazing resources on the internet for all of the aforementioned topics,
I won't be doing a deep dive into any of them. Rather, I'll explain the basic concept and show a few relevant code
examples if necessary, and then link to further reading on the topics. Over the past few years, I've bookmarked and
curated great examples, code snippets, and videos that were instrumental in my learning and that I would love to pass on.

I'll use an emoji system to give more context as how necessary / important it is that you review said resource.

:fire: : Must read or watch, extremely valuable and explains key concepts.

:star: : Good to know but not absolutely necessary. Definitely adds more context.

:sparkles: : Not directly relevant but still very interesting. If you have some extra time, you can work through this.

So, without further ado, let's level up!

## Table of Contents

1. [Higher Order Functions](#higher-order-functions)
1. [Functions as First-Class Objects](#functions-as-first-class-objects)
1. [this keyword](#this-keyword)
1. [Prototypical Inheritance](#prototypical-inheritance)
1. [ES6 Classes](#es6-classes)
1. [The Event Loop](#the-event-loop)
1. [Promises](#promises)

## Higher Order Functions

## Functions as First-Class Objects

## `this` keyword

## Prototypical Inheritance

## ES6 Classes

## The Event Loop

JavaScript is really fast when it comes to IO (input/output) and pretty slow when it comes to CPU intensive tasks.

In other words, JavaScript is great when you need to communicate with other computers. The classic example is a chat app.
You need to send and receive a large volume of relatively small messages and you need to process them quickly.
JavaScript excels here.

On the other hand, if you're trying to do intensive math calculations,
JavaScript is going to be really slow for a few reasons, one of which is that you're restricted to a single thread.

I won't dive into what threads are (see below for additional reading). The key point here is that because
JavaScript is a single-threaded language, **it can only ever do one thing at a time**. But, if it can only ever do one "thing",
where we might consider a "thing" to be a function call, then why is it so fast?

The answer lies in JavaScript concurrency model AKA the **Event Loop**.

A brief aside on concurrency, a very simple definition of concurrency
is the ability of a system to start, stop, and switch between tasks while in the middle of their execution i.e.
the ability of a system to multi-task.

Humans are actually really good at concurrency.

Consider a chef preparing a three course meal. If the instructions for the entree say to roast a chicken for two hours,
the chef isn't going to sit and wait for the chicken to finish roasting AND THEN move on to any other steps or dishes.
Rather, the chef will put the chicken in the oven, move on to some other tasks, and when the chicken is done the chef
will be _called back_ to the oven to remove the chicken.

Notice what the chef is doing (and the hopefully obvious reference to `callback` functions). The chef _starts_ roasting
a chicken, the chef _starts_ cutting up vegetables, the chef is notified that the chicken is done roasting so the chef _stops_
their current task and _resumes_ chicken preparation. The chef is constantly starting, stopping, resuming, and switching
between tasks. The chef knows to return to a task when they're _called back_ or notified to resume it.

So with this in mind, the **Event Loop** then is the mechanism by which JavaScript is able to quickly start, stop,
resume, and switch-between tasks.
Note that it's entirely possible for tasks to execute in an order that isn't the same as what you might expect
when reading a file from top to bottom.

### Resources

## Promises
