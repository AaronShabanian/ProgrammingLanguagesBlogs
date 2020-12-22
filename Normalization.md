# Normalization
In this blog I will go over Normalization and abstract rewriting. Normalization is the act of simplifying a abstract function until it is said to be in normal form. 
We know a function is in normal form when it can no longer be normalized or reduced. In other words, it can't be re written in following any of the rules. 
## Normalization example
Here is an example of normalization. 
<br>
Rules (ARS)
```
ab->a
ba->ab
```
Steps
```
babbaabbaaaab  
babaabbaaaab   ab->a
baaabbaaaab   ab->a
baaabaaaab    ab->a
baaaaaaab    ab->a
baaaaaaa      ab->ab
abaaaaaa      ba->a
aaaaaaa       ab->a
Final Answer: aaaaaaa
```
As can be seen in this example, our answer is in normal form. We can say it is in normal form due to the fact that it can no longer be simplified according to the rules that are 
mentioned above. This can also be said saying that it is irreducable. 

## Basic Notation
There a couple different basic notations that are necessary to be known to reduce a function. 
<br>
We should know that = is the identity relation, -> is the smallest preorder. We should also know that them together should be the transitive closure.

## Confluence
From abstract reduction systems we should know if an ARS is confluent or not. We can define confluence by if x reduces to y and z and y and z are joinable. Our above example is 
confluent since it does not have an infinite loop and it does follow the definition of confluence. An example of one that is not confluent is:
``` 
ab->ba
ba->ab
```
This is not confluent due to the fact that it is an infinite loop. 
