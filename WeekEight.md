<h1> Abstract Reduction Systems (1/2) </h1>
Main Source: https://hackmd.io/@alexhkurz/Hymy2npDS

We will be going over the basics of what an ARS is, as well as learning about Confluence and Normal Forms 
<h3> Introduction </h3>
Important things to remember before diving into ARS:
- The order in which rules are applied should not matter
- The golden standard is to:
  - Understanding the computation with the order that looks easiest
  - Then applying the order that runs the fastest 

<h3> ARS: Models of Computation </h3>
Definition: An abstract reduction system (ARS) is a set A together with a relation -> →⊆ A × A.

- elements of A can be any types of elements: numbers, strings, lists, trees, etc. 
- a∈A is a normal form if there is no (a,b)∈→, or, if there is no a→b. 
