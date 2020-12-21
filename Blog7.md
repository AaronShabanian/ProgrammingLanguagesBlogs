# Modules
## What Are Modules
This semester we learned about typical Haskell syntax but never really went over Haskell modules. Modules in haskell are very similar to the way packages work in both python 
and Java. For example, in Java you can import 'Java.util.*' that allows you to do operations on many differeby utilities such as arrays and arraylists. Python has similar types
of packages that can be installed with pip and can be imported into specific scripts. One example of one of these modules is NumPy. NumPy allows the script to do complex math 
equations without doing anything special. Modules in Haskell operate in a very similar way to all of these. 
## Syntax of modules in Haskell
In Haskell you can use `import modulename` to import modules. You can import both premade modules or you can make your own modules and then import them. While the syntax to 
import pre made modules is relatively simple, it can be a little harder to make your own custom module. Below, I show an example of how to create a custom module that can be 
used in Haskell. 
```
module Custom(
  checkEven
) where
checkEven:: Int-> Bool
if x 'rem' 2 == 0 
   then True 
else False 
```
This custom module only consists of one function but modules could contain as many functions as we wanted. To use this function we would do 
```
import Custom 

main = do 
   print(showEven 4) 
```
This function should return true as we made this method in our module. 
## Benefits of Modules
Using modules can have a plethora of benfits. First of all, it can help lower the actual amount of code you have to write since you could have a big amount of functions that 
are already written. Second, it can help you when you don't really have the knowledge of how to write a specific block of code. For example, you can use our above module to see
if a number is even even if you don't know how you would make the code to do that. 
## Examples of Pre made modules
Some common premade modules are the List module, Char Module, Map Module and Set modules.
### List Module
The list module allows you to perform different operations on lists such as spliiting it up and sorting it. 
### Char Module
The char module has predefined functions that can help you work on chars such as toUpper and toLower that allows you to change the case of the character from capital to 
lowercase and from lowercase to capital. 
### Map Module
The map module creates a new datastructure thats similar to a hashmap thats used in other programming languages. 
### Set Module
The set module creates sets that are similar to arrays but all elements are unique. It does this by using a binary tree
