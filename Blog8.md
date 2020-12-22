# Monads
## Overview
We know that monads are a type of applicative functor that have extra features. Monads can also be described as a type class which are governed by 3 rules that are called monadic
rules. <br>
The three basic rules are: 
<br>
Left Identity Law - Where the value in the return function does not change and it should not change anything in the Monad. 
It can be written as 
```
return >=> mf = mf
```
Right Identity Law- Has the same definition of the left identity law where the value in the return function should not change and nothing in the monad should be changed. 
It can be written as 
```
mf >=> return = mf
```
Associativity- Functors and monads should work in the same way. It can be expressed as: 
```
( f >==>g) >=> h =f >= >(g >=h)
```
## Monad example
An example of a monad declaration can be seen below
```
class Monad m where  
   return :: a -> m a 
   (>>=) :: m a -> (a -> m b) -> m b 
   (>>) :: m a -> m b -> m b 
   x >> y = x >>= \_ -> y 
   fail :: String -> m a  
   fail msg = error msg 
```
All three rules can be seen in the above example. The Right identity, left identity and associativity rule can be seen above in the example aswell. 
<br>
We can also use a monad to generate a specific list. We can do this with this example. 
```
print([1..10] >>= (\n -> if even n then [n*2] else []))
```
This would return a list with these numbers as it multiplies all the multiplies all the even numbers by 2 and deletes all the odd ones
```
[4,8,12,16,20]
```
Overall Monads have many uses and can help in the development process. 
