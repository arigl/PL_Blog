How Haskell compares to other programming languages through my perspective:

The most interesting part of this course so far is diving deep into Haskell, and discovering how you can apply the fundamental knowledge of a programming language such as this one to better understand others. Working with Haskell made me have a much deeper rooted apprciation for type mismatching and how easy it is to work on in a more robust modern programming language.

For Example:
In order to convert a float to an integer its pretty simple in most programming languages.
Simply cast a float as an Int and you are pretty good to go.

float y = 1.4
int x = (Int) y
Output -> 1

However in Haskell, You need to think more strategically.
First you would need to separate the float into a fraction, as a pair, then take the first value of it possibly as a natural number.
Then after obtaining the first value, you would need to convert it into an integer with its own recursive functions.

Simply doing one thing automatically turns into a chore in Haskell where you need to go through multiple functions to reach an end goal. 
Discovering and learning this was very interesting, but for the most part just makes me appreciate common programming languages I work with more for their ingenuity and ease of use.
