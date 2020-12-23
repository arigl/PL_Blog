<h1> Midterm Review </h1> 

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
You can't remove Bs.
```

<h3> Opinions of the exam </h3>

Overall I felt like the exam was pretty fair, but I could have used more time. I definetly felt like I spent a lot of time studying for this exam, even compared to my peers who scored higher than me, but that could be due to my exam taking abilities, which is something I have always been bad it. Question 1 is a really nice way to ease into the exam, as simply having this question on this exam helps to reinforce the ideas of some of these definitions in your head. Overall Question 2 could have been a lot better for me, and if I were to give a reccomendation it would be to choose a problem that does not have more than 5 or 6 equivalence classes. Having 9 equivalence classes is just very difficult to process through on a timed test, especially in an online format where I would argue time matters even more due to the added factor of having to make a pdf with all of your pages and turning it in time. Number 3 was a good question overall, I would have gotten this right if I just spent maybe 15 or 20 minutes more studying this specific portion. Number 4 was also a fair question as well.

I felt like the exam was challenging but overall very fair with the questions given. I did not think it would be this similar to the practice test, and maybe if this was your intention to make it more clear to the students. I went through every single lecture notes trying to learn every small detail, which helped a lot in understand the class but it did not help me on the exam. 
