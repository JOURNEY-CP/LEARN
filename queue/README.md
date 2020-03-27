# QUEUE

## THEORY
You have seen queue at many places. The data structure queue is also similar to this.
FIRST IN FIRST OUT -- the one ehich comes first leaves first..
main methode in it
- ENQUEUE  adds 1 element to QUEUE at last
- DEQUEUE  deletes 1 element from QUEUE from front
- SHOW_FRONT to return the first element of QUEUE without rempving it

## IMPLEMENTATION USING C++ STL

### HEADER FILE
```
#include<queue> 
```
if You use ```#include<bits/stdc++>``` then the above one is not needed

### initiating 
In your function where you want to use you want to do like 
```
void myfun(){

	queue <int> Q;

}
``` 
Here Q is a the object of type _queue_ we will use this Q in further.
### check for Empty ness
```
Q.empty()
```
if Queue is empty this returns True else False
### ENQUEUE
to enque we want to push it
```
Q.push(5);
```
### DEQUEUE
to dequeue we want to pop
```
Q.pop();
```
but before this we want to check wether QUEUE is empty or not.
if Empty we cannot pop
so the code is
```
if(!Q.empty())
	Q.pop();
```




*we cant do like this*
```
P=Q.pop();
```
this gives a  error

### SHOW_FRONT
the front method returns a referance to the first element
```
if(!Q.empty())
	std::cout<<Q.front();
``` 
*dont forget to check the emptiness of QUEUE*

These are the basic methods in queue
but stl offers even more they are

### show_back
to acces the last inserted element
```
cout<<Q.back();
```
here I neglected but check for emptiness always..

### size
```Q.size``` returns the size of QUEUE