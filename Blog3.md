# Week 3 Blog
This week we continued to learn more about Haskell and its syntax while going more in depth to specific functions for our calculator assignment. We learned how to use different
data types such as natural numbers and positive numbers while learning how to write it in code. For homework we were given tasks to create different functions such as add one and 
minus one. Learning abstract syntax was an interesting subject as most of my prior programming experience was written in concrete syntax. An example of abstract syntax can be seen
below 
```
add (S O) (S O)
```
compared to concrete syntax:
```
num1+num2
```
The difference of this might seem minimal when written, but the abstract syntax allows you to further understand functions that you are using and writing as it requires you to 
completely understand the function before it is written as we had to write the basic operator functions ourselves before we could implement them to make other functions. For 
example, before we could write a full gcd function, we had to write our own mod function as gcd would use that. Both Functions can be seen here
```
modN :: NN -> NN -> NN
modN n O = O
modN O n = O
modN n m =
  if n == m
    then O
    else if less n m
      then n
      else modN (subtr n m) m

gcdN :: NN -> NN -> NN
gcdN O O = O
gcdN O y = y
gcdN y O = y
gcdN x y = gcdN y (modN x y)
```
