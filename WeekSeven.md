<h1>Semantics of Lambda Calculus:</h1>
This post is mainly suited to understanding the semantics Lambda Calculus, as well as understanding examples of programs that could be on the exam
Primary resource: https://hackmd.io/@alexhkurz/H1e4Nv8Bv#Solution-to-selected-Exercises

<h2> Overview </h2>
The main ideas to understand in this section is:

- Substitution
- Understanding a function with two arguements 
- The β-Reduction rule
- Understanding name ruling 

<h2> Understanding Substituion </h2>

The example that we will be using to understand various fundamentals is:
```
f(x)= 2 ∗ x + 1
```
If we were to substiute 3 into the equation it would look like this:
```
f (3) -> 2 * 3 + 1
```
Now if we were to convert this into lambda calculus, it would look like this: 
```
(λx.2 * x + 1)3 -> 2 * 3 + 1
```
If we refer to the basis of lambda syntax we see that 
```
- x = the variable we will be adjusting 
- e = 2 which will be multiplied with the number outside of the parenthesis, 3
```
Why is this important?
```
Substiution allows us to make placeholders within lambda calculus, and minimize long functions into regonizable pieces.
It is the basis of applying complicated functions to lambda calculus, and allows us to deduce functions to its foundation. 
```

<h2> Function with Two Arguments </h2>

A function that adds two numbers can be written as 
```
λx.λy.x + y
```
and when we add the previous example, it appears as 
```
(λx.λy.x+y)2 3
```
Then when we consider the rules for parentheses, which will help us with substiution..
```
((λx.λy.x+y))2) 3
```
<h3> Inner Substiution </h3>
We can apply inner substiution by applying the substution twice.  
```
((λx.λy.x+y)2 -> (λy.2 + y)
```
After applying inner substituion (everything in the first parenthesis), we can apply the second variable 
```
((λx.λy.x+y))2) 3 -> (λy.2 + y)3
                  -> 2 + 3
```
