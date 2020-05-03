# MAP

Map i.e., Hash Table is a data structure which stores mapped values of given key values, map Library in c++ is somewhat similar to dictionary in python 

Some basic functions of map are insertion of key-value pair,deletion of given key value,iteration of data structure
## HEADER FILE
```#include<map>```
## INITIATING
- mapping of integer keys to integer values
	```map<int,int> m;```
- mapping of string keys to integer values
	```map<string,int> m;```

## OPERATIONS
- Insertion :
 ```m.insert({key,val});```
- Deletion :
 ```m.erase(key);```
- Iteration :
```
for(auto it=m.begin();it!=m.end();++it){
	cout << it->first << ' ' << it->second << '\n' ;	
}
```
  Note : In the above code , the keyword auto automates the task of determining the suitable data type of variable it , the data type of "it" is an iterator to stl::map i.e., 
  ```map<int,int>::iterator```. It does so in compile time , hence not effecting run time of program .
  ```it->first``` : key , ```it->second``` : mapped value of given key
  one key can never map to 2 different values
- Accessing mapped value :
   	```cout << m[key] ;```
- Size of Hash Map :
	```cout << m.size() ;```
- Check if a key is present in map :
 	```m.find(key)``` returns ```m.end()``` if key not present in map else iterator to key is returned
 	
## Time Complexity
Insertion , Deletion , Accessing mapped value take O(log N) time as hash map is implemented using balanced binary trees

## practice
For a better understanding try solving [this problem](https://practice.geeksforgeeks.org/problems/twice-counter/0)
Though this might be solved by some other techniques , try solving this using hash maps
# [go to all topics](https://journey-cp.github.io/LEARN)