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
   -> bbbaaa
   -> bbabaa
   -> babbaa
   -> abbbaa
   -> abbaba
   -> ababba
   -> aabbba
   -> need to finish 
```

<h2> Termination </h2>

