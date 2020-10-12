Understanding Natural Numbers in Haskell:

The foundational units of numbers within programming languages are typically: Int, Double, and Floats 
However, in a deeper language such as Haskell, most integer types consist of either Natural Numbers and Positive Numbers 

In our example, the natural numbers data type is formatted as follows:

data NN = O | S NN
    deriving (Eq,Show)
    
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

