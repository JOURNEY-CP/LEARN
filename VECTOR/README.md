# < vector stl>

## what  is vector?
- vector is a linear data structure.
- unlike stack and queues here u can access any element you want.
- it is like arrays .
If there are arrays then why a vector?
## problems with arrays:
1. memory management. 
2. writing codes for deletion , insertion etc.. for  an element in an array.
## How vector overcomes this??
1.memory management:
    it uses dynamic arrays.
2.writing codes for deletion ,insertion  etc.. an element in an array.
    we have predefined functions in vector stl.

## How to use vectors?

## 1.How is a vector defined?
vector is a template which is included in stl 

template:
```
vector<int> v1;
vector<char> v2;
vector<string> v3;
```
- above described v1,v2,v3 represents " structures". 
- we know that structures can contain variables ,functions etc.. which can be public or private.
- we also know that we can access these using dot representaion like ```v.a``` (this gives a varible  which is included in structure v).
- ```v.b()```(this calls the function b which is include structure v).
- thus vector acts as a template or a container class by specifying the type u want like int,char etc .. it provides you structures.

How to use vector in your program:
```#include<vector> ```

intiallizing vector to get a structure;
intialise the respective data type which you want as 
```
vector<int> v1;
vector<char> v2;
vector<string> v3;
```

## 2.functions included in a vector stl?

```v.push_back(a)``` to add element to the vector at end.

```v.size()```for finding size of v.

```v[i]``` or ```v.at(i)```for acessing element at position i.

"itr" mentioned below is an iterator.iterator is a pointer to element in the structure;
```vector<int>::iterator itr;```

iterator  initilzation  
```itr=v.begin()```here it points to starting element of a vector.

 ```v.insert(itr,a)```inserts element a at position itr.
```v.erase(itr)```erases the position representing itr or deletes element \*itr . 

```v.erase(itr1,itr2)``` erases  the positions from it1 t0 it2.



## *WITH USING VECTORS WE CAN IMPLEMENT STACK AND QUEUE* _FIND HOW??_

[go to all topics](https://journey-cp.github.io/LEARN).
