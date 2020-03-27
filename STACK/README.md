
# STACK

## THEORY
A stack is a container of objects that are inserted and removed according to 
LAST-IN-FIRST-OUT(LIFO).. i.e last inserted element comes out first ,
elements can be added and removed from the stack only at the top of stack.
stack has 2 main operations:
### PUSH(x)---->adds an item to the top of the stack.
### POP(x)----->removes item from top of the stack;
some important applications where stack is very useful:
### checking validity of balancedparanthesis.
### reversing of string.
### infix to postfix.

## IMPLEMENTATION USING C++ STL

### HEADER FILE
```
"#include<stack>"
it is necessary whenever you use <iostream>
if <bits/stdc++.h> is used it is not necessary.
```
### main()
```
stack <int> s;
```
in main() ,first we declare stack as 
stack <int> s;
i.e now stack named as s is created.

### functions:

#### isempty() 
```
return s.empty();
```
 ..return 1,if s is empty.
 ..retun 0,if s is notempty.
 
#### push(x) 
```
s.push(x);
```
inserts element x into top of stack s.

#### pop()
```
if(!isempty()) 
{
s.pop();
}
```
deletes element from top of stack s.
above if condition is important bcoz if stack s is empty there is no element to delete,
so if we didnt write if(!isempty()) condition we ill get runtime error.

#### top()
```
if(!isempty())
{
s.top();
}
```
returns the topmost element from stack s.
same as pop here also above if cond is necessary as if stack s is empty,
 there is no topmost element.
 

