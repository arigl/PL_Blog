<h1>Understanding Natural Numbers in Haskell:</h1>

The foundational units of numbers within programming languages are typically: Int, Double, and Floats 
However, in a deeper language such as Haskell, most integer types consist of either Natural Numbers and Positive Numbers 

In our example, the natural numbers data type is formatted as follows:
```
data NN = O | S NN
    deriving (Eq,Show)
```    
Now we can begin to break each part down:
- data NN declares this block of code as a data type, with O as a base case and S NN to augment that
- This data type is derived from (Eq,Show) which form the basis using prestablished Haskell libraries, which we don't need to focus on for now.
- The first thing to understand is O.
  - O is classified as the starting point, or its initialization. This functions as a 0, signaling the beginning.
  - S NN is classified as an additional unit, therefore if S exists once, then it could be understood as 1.
  
Now that we have broken down what each part means, we can go into why this is useful and how to utilize this information. 
In order to build functions from this data type, we will use the fact that O is classified as 0, and that S attached to O is classified as 1, to make mathematical formulas.

Lets take argueably the most basic function, addition, as a starting point. 
The addition function follows this format: NN -> NN -> NN
This simply means, two natural numbers are taken in as inputs, and one NN will be the final output.
In simple terms this is the same as 1 -> 1 -> 2, when plugged into a formula we will create.

We first need to establish a base case, where if 0 is added to another natural number, it will simply equal the original natural number.
- The first step is to call the function:
    - add
- The second step is to establish the case, for this case we wanted to determine what happens when the number is O, or 0
    - add O 
- The third step is to determine the natural number, we initalize the number with n, but you could use any variable name.
    - add O n =
- Finally, we want the output to be n, because n + 0 is simply n
    - add O n = n 

Now that we have our base case, we need to determine what happens when a natural number that is not O (or 0), is entered as an input.
We need to implement recursion, so that the function is constantly called until each number is added one at a time, for instance if the inputs are 2 and 5, it will be called 7 times.

```
To do this, lets set up the general format:
- The first step is to call the function on both sides.
    - add () = (add)
- Next if we recall that S attached to a natural number, (n) in this case, is determined as 1, then we should use that as the base identifier to add 1 each time.
    - add (S n) = S(add n)
- Now we want to actually add with the other variable, we utilize m, on both sides of the equation
    - add (S n) m = S (add n m)
```
Now we have a perfectly working additional function with natural numbers as follows.

```
-- addition
add :: NN -> NN -> NN
add O n = n
add (S n) m = S (add n m)
```

This was a very basic and simple guide going over natural numbers, use this as a basis to work on other functions such as multiplicationa dn subtraction, which use very similar methods to reach the final product. 
