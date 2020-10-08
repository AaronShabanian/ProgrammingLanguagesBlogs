# Week 2 Blog
In week 2 of class we continued to learn Haskell Syntax and how to write basic functions such as addition and subtraction. In this blog I will compare a basic function such 
as gcd in Haskell to those in Python and benchmark the differences. The basic addtion function in Haskell can be seen below

```
gcdN :: NN -> NN -> NN
gcdN O O = O
gcdN O y = y
gcdN y O = y
gcdN x y = gcdN y (modN x y)
```
This can be compared to the addition function below in python
```
def gcd(a, b):
    while b:
        a, b = b, a%b
    return a
```
<h2> Elegance/ Structure </h2>
Just by looking at these 2 functions we can see some differences. For example in python, rather than use recursion, a while loop is used to keep going until an answer is found.
However, in Haskell there is a recursive call at the end of the function until one of 3 conditions are met.  
<br>
<h2> Time Complexity </h2>
Looking at the time complexity of both of these functions, they are both O(n) because they are both looped through (n) times until an answer is returned. Because of this, there 
looks to be be no inherent difference or advantage of the Haskell or Python function to be used. 

<h2> Benchmarking </h2>
Based on the run times of both the python and Haskell functions, they are both extremely small, but are fairly similar which what was expected since they both have very similar 
time complexities, 
