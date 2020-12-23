<h1>Why learning Haskell and other functional programming languages is important.</h1>

My first thought going into Programming Languages was that it would be another theoritical class I wouldn't use. Often in higher education, you don't really have much of a choice in what classes to take, so typically I go into the classes with the mindset of getting through it. 

However, once I began working in Haskell I knew this class would be instrumental to my programming foundation. It teaches you to view programming from a different perspective, which helps you view projects at a more fundamental level. 

Instead of simply manipulating a function you already know works, Programming Languages teaches you to view it a deeper perspective, which allows you to understand the foundational aspects more. 

By having a deeper understanding, it improves your overall programming efficiency when utilizing different functions you have a better understanding of. 

<h3> Example </h3>

One of the things we capitalized on the course was rewriting systems. The core of the functionality behind these systems is to reduce a larger string, into a smaller one following specific rules given by the function. Sometimes this can be quite daunting, the more rules you have the harder it can become harder to reduce to a normal form (in most cases this is reducing a larger string to a smaller, normal form). However, as I went through the course I thought through things more prgramatically rather than theoritically. I began to learn that the best way to solve problems is through making a program yourself, rather than trying to think through it in your head. 

For Example:

```

a -> bb
c -> d

```

This can be programmed in Java such as:

```

public static int ARS(String x){
 if(x.contains("I$I")){
    x = x.replace("I$I", "a$b");
    System.out.println(x);
    ARS(x);
 }
 else (x.contains("Ia")){
    x = x.replace("Ia", "aa");
    System.out.println(x);
    ARS(x);
 }
}

```

This also you to see every step on how a computer would reduce a normal form, and its often the easiest and leaves the least amount of room for error. 

