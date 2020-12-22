# Functors
## Regular Functors
In this blog we will learn about functors. A Functor in Haskell is a functional representation of different types that can be mapped over. It can also be seen as implementing 
polymorphism. All types are instances of functors in Haskell such as maps, trees and lists. A simple example of a functor can be seen as: 
```
class Functor f where 
   fex :: (a -> b) -> f a -> f b 
```
In this functor, a function is taken and a different function is returned. <br>
An example of using a functor is below
```
print(map (add 1) [1,2,3,14])  
```
This would return the following result. 
```
[2,3,4,15]
```
## Applicative Functors
An Applicative functor is a regular functor with some extra features. The features are from the Applicative Type class. The definition of the applicative functor is as follows.
```
class (Functor f) => Applicative f where   
   pure :: a -> f a   
   (<*>) :: f (a -> b) -> f a -> f b  
```
One module from the Applicative type class is the control module. 

## Monoids
In a monoid we get the input as the output. For example, we would input a 2 and get a 2 as the output. An example of a monoid can be seen below : 
```
mult:: Int->Int 
mult x = x * 1 
add :: Int->Int 
add x = x + 0 

main = do  
   print(mult 9)  
   print (add 7)
```

The output of this would be 
```
9
7
```
as the input is the same as the output
