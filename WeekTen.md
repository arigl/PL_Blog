<h1> Midterm Review </h1> 

<h2> Lambda Calculus </h2>

<h2> String Rewriting </h2>
<h4> SR 1) Consider the schemes of rules </h4>

```
 ab -> ba
 ba -> ab
 aa ->
 b ->
```
Reduce the strings abba and bababa
```
abba -> baab
     -> bb
     ->  

bababa -> bbabaa
       -> bbab
       -> babb
       -> a
```
Why is the ARS not terminating?
```
The ARS is not terminating because ab -> ba and ba -> ab is an ambiguous algorithm and does not terminate.
```
How many equivalence classes does it have?
```
There are two classes because there are two normal forms. A and empty word.
{w| #a in w is odd}
{w| #a in w is even}

```
<h4> SR 2) Consider the schemes of rules </h4>
 
```
ba -> bbaa
aa -> 
ba -> ab
ab -> ba 
```

Can you reduce ab to aabb?

```
ab -> ba
   -> bbaa
   -> baba
   -> abba
   -> abab
   -> aabb 
```

Can you find a nice way of stating which words are in the equivalence class of ba?

```
Words only containing A's in an even amount can end in an empty word 
Words only containing A's in an odd amount can end with A
```

Can you list some properties of words that remain invairant under application of rules?

```
asdasd
```
<h2> Termination </h2>

