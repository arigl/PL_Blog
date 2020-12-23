<h1>Programming Languages Megathread:</h1>


Everying you need to start learning and installing Haskell!

<h3>Want to just try out Haskell?</h3>

- Online compiler and tester for Haskell
  - http://tryhaskell.org/
  
<h3>Installation:</h3>
- Preface:
  - If you have a mac or linux machine, it is HIGHLY reccommended you use that over a Windows machine. Even if it is less powerful, it will make your experience far more enjoyable as most issues I encountered with Haskell was because I was on Windows. 
- Haskell Installation 
  - https://www.haskell.org/platform/windows.html
- Choclatey Installation (needed as a prereq for Haskell installation)
  - https://chocolatey.org/install
 
<h3>Haskell Tutorial:</h3>

- Starting out in Haskell: 5 Steps
  - Start working in Haskell with begining in your termininal, and utilizing a calculator in Haskell!
  - Text Guide: https://wiki.haskell.org/Haskell_in_5_steps
- Types and Functions
  - Describes the fundamentals on how to approach types and functions in Haskell, helps you undestood how to tackle assignments
  - Video: https://www.youtube.com/watch?v=pitjnqRKyyI
- Recursion
  - Recursion is very important in this class, and allows you to tackle the first assignment's difficult way of viewing functions.
  - Video: https://www.youtube.com/watch?v=y6xiaSkVlvs

<h3>Documentation and Libraries:</h3>

- Hoogle (allows you to search up the meaning of functions and how to reference them)
  - https://hoogle.haskell.org/
- Hackage (documentations for specific types and functions)
  - https://hackage.haskell.org/package/base-4.12.0.0/docs/Data-Int.html
  
<h3>Helpful Haskell Information:</h3>

- Haskell cheat sheet (contains important syntax and functions to learn and master!)
  - https://jutge.org/doc/haskell-cheat-sheet.pdf
  
<h2> Learning about String Rewriting </h2>

Want to test your normal forms against specific rules? Use this java template. 
```
public class Main
{
     public static void main(String []args){
        ARS("$V$V$");
     }
     
     public static int ARS(String x){
        if(x.contains("x")){
            x = x.replace("x", "y");
            System.out.println(x);
            ARS(x);
        }
        else if(x.contains("x")){
            x = x.replace("x", "u");
            System.out.println(x);
            ARS(x);
        }
        // ADD MORE RULES IF NEEDED 
        else (x.contains("x")){
            x = x.replace("x", "y");
            System.out.println(x);
            ARS(x);
        }
        //System.out.println("Count: " + x.length());
        return 0;
     }
}
```
