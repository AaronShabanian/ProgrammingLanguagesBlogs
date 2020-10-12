# Week 4 Blog 
This week, we learned about concrete syntax in haskell compared the abstract syntax that we learned last week. To add something in abstract syntax, I would use the syntax: 
```
add(5,3)
```
If I was to do this in concrete syntax it would be in the form: 
```
5+3
```
To convert from concrete syntax to abstract syntax, a parser tree would need to be used to convert to abstract syntax. For our parser we used BNFC to convert concrete syntax to 
abstract syntax for our calculator assignment. An example of what a parser tree would do can be seen below. 
<br>
``` 
Concrete syntax: 4+(5*3) 
Parser
     Plus
     / \ 
  Num   Times
   |      / \
   4   Num   Num
        |     |
        5     3
Abstract Syntax: Plus(4,Times(5,3))
```
This parser helps convert what most people would consider "Normal Syntax" into a syntax that our functions in our calculator could understand since there are no symbols
in our actual calculator syntax.

A simpler parser tree example can be seen below
```
  Plus
     / \ 
  Num   Num
   |     |
   2     2
