<h1> Midterm Review </h1> 

<h2> Lambda Calculus 

<h2> String Rewriting
<h4> SR 1) Consider the schemes of rules 

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

<h4> SR 2) Consider the schemes of rules 
 
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

