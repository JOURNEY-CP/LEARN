# STL
- you can find basic functions of stl here
  
## lower_bound
Used to find lower bound of a number in array/vector etc
- ``` lower_bound(a,a+n,element);```
- ``` lower_bound(v.begin(),v.end(),element);```
- Return value:
    Iterator to the first occourance of ```element``` . If element is absent returns the iterator of a position where we assume to find it.
- usage:
    if we want position of first occourance of ```x``` in a array we can do like
    ```lower_bound(a,a+n,x)-a;```

# [go to all topics](https://journey-cp.github.io/LEARN)