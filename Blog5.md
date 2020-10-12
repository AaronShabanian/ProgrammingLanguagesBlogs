# Week 5 Blog
In week 5 of programming languages, we stepped away from Haskell and moved to Lambda calculus. our basic goals when learning lambda calculus were to understand if what we were 
reading is a lambda calculus function and to be able to construct a syntax tree from reading a lambda calculus function. The three programming constructs in Lambda ca are Abstraction, 
Application and variables. <br>
The definition of the abstract syntax in Lambda calculus is ```e:: = λx.e ∣ ee ∣ x ```. <br>
When writing Lambda calculus functions, the format takes in the function and the argument side by side in the format 
```
(\x. x+1) 2
```
Just like in week 4, we used BNFC to convert concrete syntax to abstract syntax. The BNFC syntax for lambda calculus is as follows 
```
EAbs.   Exp ::= "\\" Ident "." Exp ;  
EApp.   Exp ::= Exp Exp1 ; 
EVar.   Exp1 ::= Ident ;

coercions Exp 1 ;
```
We also learned about substitution in Lambda caculus. For example, we could have the example, 
``` 
f(x)=3∗x+2

where x can be subsituted for x=4 to get 

f(x)=3∗4+2
```
This same concept can be brought into a lambda calculus expression such as 
```
(λx.λy.x+y) 2 3
to become
(λy.2+y) 3
```
Learning the syntax and substitution rules can be a valuable tool in learning Lambda Calculus and can help understand more of the basics in programming languages. 
