<h1>Syntax of Lambda Calculus:</h1>
This post is mainly suited to understanding Lambda Calculus, as well as exploring examples that may be useful on the exam. 


Primary Resource:
https://hackmd.io/@alexhkurz/S1D0yP8Bw

<h2> Overview </h2>

```
Lambda Calculus has three constructs
- Abstraction
  - Basis: λx.e
  - Components:
    - e: is a program
    - x: is a variable
    - Basis: program (or function) which as a formal parameter of x
    - This is known as an abstraction because the basis does not depend on the variable x anymore 
- Application
  - Basis: e1e2
  - If e1 and e2 are programs, then the basis is teh program which applies e1 to e2
- Variables
  - The basic programs are just variables 
```

<h2> Abstract Syntax </h2>

```
- Basis: ::=λx.e∣ee∣x
  - Where x ranges over an infinite set, the elements of which are called variables
  - If this were written in C it would look like: int plus_one(int x) {return x + 1}
- λx.e and λy.e' mean the same thing
  - Same as: int plus_one(int x) {return x+1} and int plus_one(int y) {return y+1}
- Explanation: 
  - This is because x is abstracted from the basis, and does not depend on x. Therefore, if e' arises with y replacing x, it does not change the function 
```

<h2> Concrete Syntax </h2>

Basis: similar to Abstract, but written differently for BNFC 
``` 
EAbs.   Exp ::= "\\" Ident "." Exp ;  
EApp.   Exp ::= Exp Exp1 ; 
EVar.   Exp1 ::= Ident ;

coercions Exp 1 ;
```

Syntax Explained:
```
  - λ = \
  - \\ is used to denote \ in BNF 
  - Exp :: = Exp Exp1 is used in the same way as Exp :: = Exp + Exp1 
```

<h2> Example Problems </h2>

