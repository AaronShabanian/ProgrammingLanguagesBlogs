# Week1 Blog
In the first week of clases we were introduced to basic Haskell functions and learned how to install Haskell on to our computer. On day one of classes we learned about the 
difference between imperitive and functional programming languages. As all programming languages I have learned up to this point such as C++, Java, Python and C# are imperitive
languages, functional programming languages were a new concept for me to understand. In a functional programming language such as Haskell everything is an expression rather 
than statements. This makes the computational model a lot more simpler than it is in impertive programming languages such as Python and Java. In the first week we also were given
instructions on how to install Haskell which can be seen below. 
<br> 
```  
Download Choclatey on your windows machine

choco install haskell-dev

refreshenv
```
Later in the week we learned more about basic Haskell Syntax such a creating functions, creating lists and basic recursion. The basic syntax for a function has no indentation 
and determines the input and output neccessary for each functions in this form: 
```
NN->NN->NN
```
We also learned about the syntax of basic recursive Haskell functions that re call their own existing functions such as done in python
```
fib 0 = 0
fib 1 = 1
fib n = fib (n-1) + fib (n-2)
```
If this was done in python it would be in a similar form like this 
```
def Fibonacci(n):
    if n<=0:
        print("Incorrect input")
    elif n==1:
        return 0
    elif n==2:
        return 1
    else:
        return Fibonacci(n-1)+Fibonacci(n-2)
```
As we can see it is a lot more efficient in Haskell to write as there are less if statements and the approach to writing the function is more intuitive. 
<br>
Overall this week we learned a lot about the basic fundamentals of functional programming languages, got haskell installed on our computer and started learning Haskell Basics
