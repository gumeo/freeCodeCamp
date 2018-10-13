---
title: Control Statements in R
--- 
## if/else

1. Simple if else statment

 The syntax for the `if/else` control statements in R is

    if(TRUE){
      print("Hello!")
    }else{
      print("This will never be printed...")
    }
   
2. else if

  If we need more cases, then we can use the `else if` statement
  
    i <- 3
    if(i == 3){
      print("Hi 3")
    }else if(i == 2){
      print("You are not 3")
    }else{
      print("if i is not 2 or 3, this is printed")
    }

3. Comparison operators

  You can put anything into an if statement that returns `TRUE` or `FALSE`. The commonly used operators are `!=`, `==`, `<`, `>`, `<=`, `>=`.
  
  **Note:** Since `<-` is an assignment operator in R, try to make it a habit to use spaces around comparison operators in if statements. Try to run this code and see what happens:
  
    i <- 3
    if(i<-4){ # We wanted to check whether i was less than -4, but we assign it the value 4
      print("This is weird!")
    }
    print(i) # prints 4

## for loops
  We can iterate over any object that can be indexed, e.g.
  
    > charVec <- letters
    > charVec
     [1] "a" "b" "c" "d" "e" "f" "g" "h" "i" "j" "k" "l" "m" "n" "o" "p" "q" "r" "s"
    [20] "t" "u" "v" "w" "x" "y" "z"
    > for(i in charVec){
        print(paste0(i,'_test')) # paste0 concatenates strings
      }
    [1] "a_test"
    [1] "b_test"
    [1] "c_test"
    [1] "d_test"
    [1] "e_test"
    [1] "f_test"
    [1] "g_test"
    [1] "h_test"
    ...
  
  It is also simply and conveniant to iterate over a range
  
    for(i in 1:100){
      print(i)
    }
 
  
    
  
  
  
  
  
  
