---
id: "b00a4fcc-338d-450a-958c-d6a6b2f8ae52"
title: What is declarative programming?
author: "Mark Carrier"
date: 2020-07-30
urls:
    - "what-is-declarative-programming"
tags:
    - Software
    - Draft
indexed: true
published: true
---
You can find the definitions online pretty easily. It boils down to something like this:

**Imperative programming**
> You tell the machine things that you want it to do.

**Declarative programming**
> You tell the compiler things that are true.

But it might still not be clear to you. Or at least not practical. Let's look at an example: calculating the Fibonacci sequence.

Here's my imperative version in JavaScript:
```
function fibonacci(n) {
    if(n <= 1) {
        return n
    }

    let previousValues = [1,1]
    for(let i = 2; i < n; i++) {
        const next = previousValues[0] + previousValues[1]
        previousValues[0] = previousValues[1]
        previousValues[1] = next
    }
    return previousValues[1]
}
```

Here's the declarative version from the Haskell wiki:
```
fib 0 = 0
fib 1 = 1
fib n = fib (n-1) + fib (n-2)
```

I expect the first version to feel familiar to you:
> Hello computer. I want you do this over and over again until this happens. Then stop and send the information back.

The second version just "declares" things that are true (the "what" of the problem). _Nothing_ else. There's nothing that says "how" to use the information. It's even devoid of any real sequencing. In a proper functional language, you can change the order of statements without affecting program output. You're just stating (declaring) some facts and letting the compiler worry about their relevance. 

You might think: well that's nice and all but it'll eventually need to become "real code" that the machine can actually execute. You're completely right. Declarative code isn't useful unless it's converted into imperative instructions for your processor.

The functional world's conviction is that programmers should **not** be the ones doing this. This is true for the vast majority of software problems. There's two really good reasons for removing the "how" from our code and focusing on the "what":

1. As programmers, we can focus more on our clients' problems and less and technical details.
2. We can give our compilers freedom to create imperative instructions that are likely to be better than our own.

You could think that placing this burden on compilers is complex and impractical but it isn't. It's actually quite simple.

Declarative statements can usually be converted into imperative instructions very easily. A good example of this is the `map` function. Say you wanted to get the length of each word in a sentence. The imperative version might look like this:

```
function getWordLengths(sentence) {
    const words = sentence.split(" ")
    let wordLengths = []
    for(let i = 0; i < words.length; i++) {
        wordLengths.push(words[i].length)
    }
    return wordLengths
}
```

Using `map`, you can get something more declarative:

```
function getWordLengths(sentence) {
    return sentence.split(" ").map(word => word.length)
}
```
**Look ma, no loops!**

It's trivial for a compiler to turn this into a loop if it needs to. Most of the loops we write are quite unremarkable. Why write them ourselves if the compiler knows how to handle it? It's just unneeded verbosity. Furthermore, we're actually depriving the compiler of an opportunity to perform some clever optimizations, not to mention making our code harder to read.

As beginners we might feel like declarative code is actually harder to read. There's a couple of reasons for this. First of all, more concise code means greater information density. With a little bit of practice we can get used to this. Once the training wheels are gone you'll never want to go back.

The second reason is that we're used to thinking in terms of "the machine did this and then it did that". It is a nice mental model for helping us turn something abstract into something tangible. The problem with this approach is that it's deceptive. Unless you're programming in C or assembly the machine probably didn't do what you expect. Interpreted languages (Java, Python, JavaScript, C#, etc) are doing [all kinds of things](https://dzone.com/articles/java-on-steroids-5-super-useful-jit-optimization-t) to turn our instructions into better instructions. _Even_ if you're writing C or assembly, the CPU's internals are interfering in all kinds of ways to make you **feel** like you're working with the Von Neumann architecture [despite the limitations of this model](https://en.wikipedia.org/wiki/Von_Neumann_architecture#Mitigations).

So, a revised definition of the two models could be as follows:

**Imperative programming**
> You tell your compiler things that it'll pretend to do because that's how you trained your brain to write code.

**Declarative programming**
> You tell your compiler things that are true and let it figure out the best way to turn it into something practical.

## Conclusion
As software evolves, it's logical to expect new abstractions that allow programmers to focus more on problems and less on implementation details. In most cases we're willing to sacrifice lots of performance for these abstractions since programmers cost a lot more than computers. My prime motivation for learning [FP](https://en.wikipedia.org/wiki/Functional_programming "Functional Programming") and [FRP](https://en.wikipedia.org/wiki/Functional_reactive_programming "Functional Reactive Programming") is to improve my productivity. What's surprising is that declarative programming can potentially offer better performance than most of the imperative abstractions that are prevalent. Imperative programming using a high level language is essentially taking the worst of both worlds.

I hope this convinces you of the value of researching and learning more about the different ways that you can use these not-so-easy concepts. Unfortunately we're far away from a world that allows us to take full advantage of all of functional programming benefits. Our very machines are built with the expectation that we will write imperative code. Despite this, functional programming still has [a lot to offer](https://stackoverflow.com/questions/128057/what-are-the-benefits-of-functional-programming). Performance just usually isn't the main benefit (yet).
