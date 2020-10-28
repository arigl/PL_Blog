<h1> Abstract Reduction Systems (1/2) </h1>
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

