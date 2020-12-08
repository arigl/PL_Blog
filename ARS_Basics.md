<h1> Abstract Reduction Systems (Basics) </h1>
Main Source: https://hackmd.io/@alexhkurz/Hymy2npDS

We will be going over the basics of what an ARS is, as well as learning about Confluence and Normal Forms 
<h2> Introduction </h2>
Important things to remember before diving into ARS:
- The order in which rules are applied should not matter
- The golden standard is to:
  - Understanding the computation with the order that looks easiest
  - Then applying the order that runs the fastest 

<h2> ARS: Models of Computation </h2>
Definition: An abstract reduction system (ARS) is a set A together with a relation -> →⊆ A × A.

- elements of A can be any types of elements: numbers, strings, lists, trees, etc. 
- a∈A is a normal form if there is no (a,b)∈→, or, if there is no a→b. 

<h4> Examples </h4>
A is the set of integers > 1and m→n is defined to hold if m>n and n divides m.

- normal forms are primes
-  normal forms are not unique
- two numbers are joinable iff they share a prime number (iff they are not relatively prime)
- all numbers are equivalent
- not confluent
- terminating

<h2> ARS: Confluence and Normal Forms </h2>
The main reason ARS is important is to understand the relationship between meaning and computation.
Both understanding how something works then finding a fast efficient solution will always be important in computer programming. 

&nbsp;

Understanding Big O run time speed is an important thing to know for this, so if you need to brush up on the different speeds and how to calculate them, here is a easy to understand video: 
- https://www.youtube.com/watch?v=v4cd1O4zkGw

<h4> Normal Forms </h4>
The big takeaway when it comes to normal forms is that it allows us to reduce a complicated list or data type to a more basic form to compare with another.
For example:

```
20112 → 02112
      → 0212
      → 0122
      → 012
122220 → 12220
       → 1220
       → 120
       → 012
```

We run this test in order to see if two data types are the same. Comparing every value would require a sorting algorithm with a relatively long Big O runtime, such as a bubble sort. However, if we build an ARS and compare normal forms it is far faster to compute. 

<h2> Conclusion </h2>
This first part is the beginning to understanding Abstract Reduction Systems. There are many ways to look at relationships between types, and in the next section we will be going over those, specifically Termination. 
