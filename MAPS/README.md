# MAP

Map i.e., Hash Table is a data structure which stores mapped values of given key values, map Library in c++ is somewhat similar to dictionary in python 

Some basic functions of map are insertion of key-value pair,deletion of given key value,iteration of data structure

```map<int,int> m``` ; //mapping of integer keys to integer values
1. Insertion : ```m.insert({key,val});```
2. Deletion : ```m.erase(key);```
3. Iteration :
```
	for(auto it=m.begin();it!=m.end();++it){
		cout << it->first << ' ' << it->second << '\n' ;	
	}
```
  Note : In the above code , the keyword auto automates the task of determining the suitable data type of variable it , the data type of "it" is an iterator to stl::map i.e., 
  ```map<int,int>::iterator it```. It does so in compile time , hence not effecting run time of program .
  it->first : key , it->second : mapped value of given key
  one key can never map to 2 different values
4. Accessing mapped value :
   	```cout << m[key] ;```
5. Size of Hash Map :
	```cout << m.size() ;```
6. Check if a key is present in map :
 	```m.find(key)``` returns ```m.end()``` if key not present in map else iterator to key is returned
Insertion , Deletion , Accessing mapped value take O(log N) time as hash map is implemented using balanced binary trees

For a better understanding try solving [this problem](https://practice.geeksforgeeks.org/problems/twice-counter/0)
Though this might be solved by some other techniques , try solving this using hash maps
# [go to all topics](https://journey-cp.github.io/LEARN)