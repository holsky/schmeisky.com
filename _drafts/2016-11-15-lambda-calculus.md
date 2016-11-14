---
layout: post
title:  Cool Stuff: Lambda Calculus
date:   2016-11-15
categories: languages

Lambda calculus is one of the things I heard of in passing during university, but never got a chance to dive deeper into. In Wikipedia's words it is "... a formal system in mathematical logic for expressing computation based on function abstraction and application using variable binding and substitution. It is a universal model of computation that can be used to simulate any single-taped Turing machine"<span title="https://en.wikipedia.org/wiki/Lambda_calculus"><sup>[<u>1</u>]</sup></span>. In my own words it is programming in mathematics.

## Lambda Calculus is made of expressions

Lambda Calculus is a mathematical system to manipulate functions as expressions. You already know one system where you manipulate expressions, namely arithmetic. In it combinations of expressions stand for the *result* of the expression, rather than the instruction to carry it out. So 

A = (x + y) * z^2 

is the compact form of writing, let a = x+y, b = z^2, let A = a * b. 

Lambda Calculus applies this idea to functions. Where you normally would write,

let f(x) = x^2 and A = f(5), in lambda calculus you write the definition and appl

Functions can be nested as deep as you want, regardless of intermediary value.

X > x2 Lx.x2 - x is a bound variable

## Is Lambda Calculus able to compute something useful?

One of the first questions that comes to mind with a new computational model is whether it is equivalent to the other ones, i.e. can the same kind of functions be calculated with it. At the time (1930s) these were Turing machines and general recursive functions, that were proven to be equivalently capable to compute "computable functions". A computable function is roughly comparable to something that could be calculated by pen and pencil; whether these actually are the computations that are interesting to humans is of course not provable. 


Church Turing Theiss: intuitiviely computable functions equal to turing compoutable functions


Lambda calculus capable of turing vice versa

Functional programming languages can be regarded as Extensions of lamda calculcusu with Input Output sde eff oiects and types 

Connections to logix Lambda calculus is a way to wtite xonstructive proofs by goving a Set of rulws how the thing to be Proben can be constructed - this can be poeefil for findi g algortitjms

## Adding data types and recursion

So how can you program in the lambda calculus and actually do something? So far we have seen only how expressions are evaluated. First off, we need recursion:

LC does not really have recursion because functions do not have names. There are (cumbersome) ways to work around this though;:
Every Lambda Term Gas a a Fixed Point and can be solved - this means every lambda Term Has an explicit Version with nö Free variables (eben recursive obes like for factoriall). 

LC does not have data types, but you can define them
Data types as Lambda Expression
P25 example for addlist in lambda

Types as Lambda Expression, eg ints and bools
Theb Check that most things still work with types
Intuitional logix and propositions are isomorphix to Lambda calculus- use whatever is suitable (Curry Howard Isomorphismus) proofs as Programm (proofs as Algorithmus)

Tjat way possible go build Type System etc
Int given
Sum types through Isomorphismus

Use logix rules for reductiob rules in lc

Eben better: you can extend lc to classical logix b adding a Term that is equivalent to adding an Axiom for proof by cobtradiction 
(Peirce's law) this Works through the Isomorphismus
The Term (felleisen' c ) is roughly equivalent to a goto or Break statement: you Input a Value and either xontinue regular Evaluation or jump to a given value

Introducing All quantifier crrates typed Lambda calcukus where We can eg guarantee that All boolean functions eventually reduce to t or f 

P 106
Forexample,Mcouldbeaslow,butsimplesubroutineforsortingalist.ThetermNcouldbeareplacementthatrunsmuchfaster. IfwecanproveMandNtobeoperationallyequivalent,thenthismeanswecan safelyusethefasterroutineinsteadofthesloweron

Train: evalutae Expression 
Evalutae Expression for list
Evalutae Expression for addlist list