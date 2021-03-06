---
layout: post
title: Cool stuff
permalink: /coolstuff/
date:   2016-10-31
categories: coolstuff
---

This is where I put cool stuff I found on the web in case Twitter ever ceases to exist.

* TOC
{:toc}

## Build a Container Engine in 20 minutes 

[This video is](https://www.youtube.com/watch?v=HPuvDm8IC-4) a walkthrough of starting to build a container system in a 20 minute talk, with an explanation of all the concepts involved (namespaces, hostname space/UTS, and a separate filesystem).

Of course it's not of practical use, but it's nice to get an idea how a container like Docker works. Here's the [finished code](https://gist.github.com/julz/c0017fa7a40de0543001) if you are impatient:

This [workshop](https://github.com/Fewbytes/rubber-docker) in Python goes even deeper with 10 levels to complete.

## Origins of Lisp

Lisp is that legendary language of fairy tales long lost. I found this [great article by Paul Graham](http://www.paulgraham.com/icad.html) on the origins of Lisp. Apparently it was not devised as a programming language, but as a formal language in a research paper to come up with an alternative to the Turing Machine. Only later because on of his grad students tried to implement it, was it possible to run Lisp programs. This is why Lisp was not concerned with machine limitations of that time (like Fortran), but was more like pure math.

An interesting point Paul Graham makes is that many features Lisp already had in 1958 are only now getting fully adopted by modern languages, these being: Conditionals, Function Types, Recursion, Dynamic Typing, Garbage Collection, Programs composed of expressions, symbol types, the AST notation and Lisp's Metaprogramming facilities (that together make Lisp metaprogramming extremely powerful).

## Why it can be effective to use Lisp

This is [an article, by Matthew Butterick](http://practicaltypography.com/why-racket-why-lisp.html) who struggled with the definition of Lisp as the language of fairy tales and wonders by most of its proponents without explaining exactly *what* makes it so good. 

The reasons are in short: Everything as an expression, everything as a value or list brings high consistency, well-written documentation written mostly by CS professors, IDE ships with language, X-Expressions to represent XML-ish data, Scribble is a powerful templating language, syntax transformations in Racket itself and easy-to-define DSLs.

## Smalltalk

http://www.cs.virginia.edu/~evans/cs655/readings/smalltalk.html

Smalltalk is one of those old languages that keep producing great ideas that everyone else copies (Object/Message-Oriented Programming, Virtual Machines, Images, Refactoring, Test-Driven Development, ...). I recently attended an interesting talk by [Nikolas Martens](http://rtens.org/) on it. The *attitude* and design rationale of Smalltalk is captured well by these quotes from the above article:

> Instead of a bit-grinding processor raping and plundering data structures, we have a universe of well-behaved objects that courteously ask each other to carry out their various desires.

They have a very compelling reason, why a programming language should be designed for us programmers, not for the computer:

> The mechanisms of human thought and communication have been engineered for millions of years, and we should respect them as being of sound design. Moreover, since we must work with this design for the next million years, it will save time if we make our computer models compatible with the mind, rather that the other way around. 

And when it comes to the rationale for object orientation as a way to model the world it gets really philosophical:

> The mind observes a vast universe of experience, both immediate and recorded. One can derive a sense of oneness with the universe simply by letting this experience be, just as it is. However, if one wishes to participate, literally to take a part, in the universe, one must draw distinctions. In so doing one identifies an object in the universe, and simultaneously all the rest becomes not-that-object

One major caveat for Smalltalk is often that it is suitable only for small projects. And yes, this is by design:

> Personal Mastery: If a system is to serve the creative spirit, it must be entirely comprehensible to a single individual.

How awesome is it that there is a language with this kind of spirit? Practically speaking the talk by Nikolas Martens gave some very interesting benefits of using Smalltalk for modern development. Most impressive was, when he first created the call for a function that did not exist, called it, and only then, in debug mode, started writing it. TDD to the max.

## Lambda Calculus

Lambda calculus is one of the things I heard of in passing during university, but never got a chance to dive deeper into. In Wikipedia's words it is "... a formal system in mathematical logic for expressing computation based on function abstraction and application using variable binding and substitution. It is a universal model of computation that can be used to simulate any single-taped Turing machine"<span title="https://en.wikipedia.org/wiki/Lambda_calculus"><sup>[<u>1</u>]</sup></span>. In my own words it is programming in mathematics.

I read a little into it using these [Lecture Notes by Peter Selinger](https://www.irif.fr/~mellies/mpri/mpri-ens/biblio/Selinger-Lambda-Calculus-Notes.pdf) and, but later I found this more accessible guide: [Lambda Calculus for absolute dummies](https://palmstroem.blogspot.de/2012/05/lambda-calculus-for-absolute-dummies.html). 

Why is this nice to know? Most functional programming languages (LISP, Erlang, Scala, ...) in some way use Lambda Calculus as the base and add things like side effects and state to become useful programming languages. So, to understand some of the design decisions in these languages it is useful to understand where they come from.

## Software Engineering Radio

[Software Engineering Radio](http://www.se-radio.net/) is a series of podcasts made by a awesome team of volunteers that interview a very broad and interesting range of industry experts on topics around Software Engineering, from very technical ones (like [Consensus in Distributed Systems](http://www.se-radio.net/2015/11/se-radio-episode-241-kyle-kingsbury-on-consensus-in-distributed-systems/)) to social/human ones (like [Recruiting Software Engineers in San Francisco](http://www.se-radio.net/2016/05/se-radio-episode-258-cody-voellinger-on-recruiting-software-engineers/)). I really like how it gives you a broader context in topics you are not very well familiar with and gives an insight into discussions by industry experts.

I have a [blog post](/engineering/2016/11/22/SE-Radio1.html) summarizing some of the learnings.

## Browser-based Presentations

[reveal.js](http://lab.hakim.se/reveal-js) is a tool/library for browser-based presentations with nice transitions that will work everywhere a webbrowser works. Is not as hard to setup *well* as Prezi or impress.js.

## Practical Typography

[This online book about typography](http://practicaltypography.com/) helped me as a technical person to make sense of all the endless CSS Stylings and HTML tags to structure a page (like this one). The author offers reasonable advice on when to use which technique to style text (i.e. typography) based on the vast amounts of wisdom in the typographer's profession and adapts it to the modern web. The book is free to read, but I paid the author something to reward making this great resource.

## GNU Coding Standards

An interesting side note I found in the [HN comments](https://news.ycombinator.com/item?id=14542938) on the different implenentations of very different complexity of `yes` . While the [Unix version](https://github.com/openbsd/src/blob/master/usr.bin/yes/yes.c) is as simple as you would expect, the [GNU version] rather complex, aligning memory pages and bypassing the standard library, to optimize for throughput. [One commenter](https://news.ycombinator.com/item?id=14543640) points out that quite often GNU programs look "odd", in order to avoid patent infringement concerns with UNIX. There is even a section in the (GNU coding standards)[https://www.gnu.org/prep/standards/standards.html#Reading-Non_002dFree-Code] to encourage this, e.g. by optimizing for speed instead of readability.

## Nerves - embedded Elixir

Elixir/Erlang is not something you usually associate with embedded system. Here is a framework that bridges the gap: 

http://nerves-project.org/

## Unsong

I somehow found this online book that was published until May 2017 and has come to a (surprising) end. It is a very entertaining read, since it contains a lot of word-play and played with my conception how the world works. In principle it is a large pun, that assumes flipped roles for science and superstition/religion, a world where everything from religion is true, while scientific laws do not uphold anymore. For example in the chapter [War and Peace](http://unsongbook.com/interlude-%D7%97-war-and-peace/), scientific facts that we consider a given through evidence are instead interpreted in a theological fashion:

```
 When a scientist says “space is infinite and full of stars”, she does not literally mean that the crystal sphere surrounding the Earth doesn’t exist. She is metaphorically referring to the infinitude of the human spirit, the limitless possibilities it offers, and the brightness and enlightenment waiting to be discovered.
```

## NASA

I am a huge fan of space and space exploration. [Spacepod](https://www.listentospacepod.com/) is a great podcast that brings you really close to what we do to explore space and brought to my attention some of the interesting stuff NASA does:

  * [Bright Spots and Color Differences Revealed on Ceres](https://www.nasa.gov/feature/jpl/bright-spots-and-color-differences-revealed-on-ceres) with a nod to fans of The Expanse
  * There is a [Planetary Defense Coordination Office](https://www.nasa.gov/planetarydefense/overview)
  * And they have an [app](https://cneos.jpl.nasa.gov/nda/), where you can practice defending earth from an asteroid using nukes

## English Language

The English language has a larger vocabulary than other comparable European languages like French or German, maybe because English speakers have more fun to play around with foreign words and use them in their own language<span title="This is the short version of the reasoning in [The Mother Tongue](https://en.wikipedia.org/wiki/The_Mother_Tongue)"><sup><u>1</u></sup></span>. For me, learning English will never top because of words like these:    


Digging deeper on apricity brings to light this interesting history: According to Merriam-Webster the word brought into English by Henry Cockeram in 1623 when he recorded (or possibly invented it) for his dictionary. However, it never really made it out of the dictionary into general use and is probably exemplary for the fate of English words that come only from single authors and not from general speech.
