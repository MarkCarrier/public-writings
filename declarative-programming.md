---
id: "b00a4fcc-338d-450a-958c-d6a6b2f8ae52"
title: What is declarative programming?
author: "Mark Carrier"
date: 2020-07-22
urls:
    - "what-is-declarative-programming"
tags:
    - Software
indexed: false
published: true
---

# What is declarative programming?
You can find the definitions online pretty easily. It boils down to something like this:

**Imperative programming**
> You tell the machine things that you want it to do.

**Declarative programming**
> You tell the compiler things that are true.

But it might still not be clear to you. Or at least not practical. Let's look at an example: calculating the Fibonacci sequence.

Here's my imperative version in JavaScript:
```
function fibonacci(stopAt) {
    let fibonacci = [0,1]
    while(fibonacci.slice(-1)[0] < stopAt) {
        fibonacci.push(fibonacci.slice(-2)[0] + fibonacci.slice(-1)[0])
    }
    return fibonacci
}
```

Here's the declarative version from the Haskell wiki:
```
fib 0 = 0
fib 1 = 1
fib n = fib (n-1) + fib (n-2)
```

I expect the first version makes at least some sense to you:
> Hello machine. While this condition is true I want you do this over and over again.

The second version is devoid of sequencing. In a proper functional language, you can actually change the order of statements without affecting program output. You're just stating (declaring) some facts and letting the compiler worry about their relevance. That's why the Haskell version doesn't need a `stopAt` parameter. Haskell won't actually calculate anything unless it's needed. Something "higher up" will need to "pull" some values from these truths and the compiler will only calculate as many Fibonacci values as are needed. 

As much as some might try, no imperative language can actually pretend be truly functional/declarative since they calculate stuff that you ask for instead of stuff that's needed. In Haskell _everything_ is lazy evaluated.

That's why the Haskell version can be so mathematically pure. You just needs to _declare_ 3 things that are true and the compiler will use those facts when (if) it needs to.

You might think: well that's nice and all but it'll eventually need to become "real code" that the machine can actually execute. You're completely right. Declarative code isn't useful unless it's converted into imperative instructions for your processor.

The functional world's conviction is that programmers should **not** be the ones doing this. They're right. Unless you're programming in C or assembly, you're not really doing this anyways. Interpreted languages (Java, Python, JavaScript, C#, etc) and doing all kinds of crazy stuff to make us **feel** like we're controlling the machine, but we're not.  _Even_ if you're writing C or assembly, you're not really in control of your microprocessor. Its internals are interfering in all kinds of ways to make you **feel** like you're working with the Von Neumann architecture [despite its limitations](https://en.wikipedia.org/wiki/Von_Neumann_architecture#Mitigations).

The most surprising part of all this is that declarative code isn't as abstract and unpractical as we might expect. Most of the imperative code we write could be expressed declaratively without giving our compilers any anxiety whatsoever. A good example of this is the `.map` function. map can be converted into a for loop very easily. Letting the compiler do it for us means that it can perform all kinds of optimizations (such as lazy evaluation). You can't do this when you program imperatively.

As convincing as this might be to you (I hope), the sad truth is that we're far away from a world that allows us to take full advantage of functional programming's benefits. Our very machines are built with the expectation that you will write imperative code. Functional programming still has a lot to offer. Performance just _usually_ isn't one of them (yet).