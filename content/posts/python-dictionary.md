---
title: 'Python Dictionary '
subtitle: Data Structures in python
category:
  - Programming
author: Anand Murali
date: 2019-10-18T09:44:05.496Z
featureImage: /uploads/about-hero.jpg
---
What are dictionaries in python?

A dictionary is a data structure in python used to store data as
key:value pairs.

Properties of dictionary are

1.Unique and single Key element 

2.Values can be anything(lists,integers etc).

3.Each key and value is sepearted using a colon(:)

4.Written inside curly braces {}

    Eg:- dict={ 1:'a',2:'b',3:'c' } # single key and single value

         dict1={ 1:['hi','hello'] , 2:100 ,3:100 } #value of 1 is a list. keys 2 and 3 have same value(100) which is fine.

         bad_dict={ 1:'hi' , 2:'hello' , 1:'world' } #this dictionary wont work as key is not unique


creating and Printing values from a dictionary

    
    Dict={}     
    for i in range(0,10):
      Dict[i]=input()
    print(Dict)

Input :-    
   
a
b
c
d
e
f
g
h
i
j

Output:-

{0: 'a', 1: 'b', 2: 'c', 3: 'd', 4: 'e', 5: 'f', 6: 'g', 7: 'h', 8: 'i', 9: 'j'}

Accessing an element from a dictionary


    Dict={0:'welcome', 1:'to', 2:'Learn', 3:'Free' ,4:'.co'}
    print(Dict[2])
    print(Dict[3])
        
Output :- 

Learn

Free

Updating Dictionary

Dictionary comes with a method called update, which can be used to add a new element to the dictionary, as well as update value of element in dictionary of a corresponding key.

Syntax dictionary_name.update({key:val})

For eg:- 
  
    Dict={0:'welcome', 1:'to', 2:'Learn', 3:'Free' ,4:'.co'}
    print(Dict)
    Dict.update({5:'new entry'})
    Dict.update({0:'changed the existing value'})
    print(Dict)


 Output:-
{0: 'welcome', 1: 'to', 2: 'Learn', 3: 'Free', 4: '.co'}
{0: 'changed the existing value', 1: 'to', 2: 'Learn', 3: 'Free', 4: '.co', 5: 'new entry'}


items()

    Dict={0:'welcome', 1:'to', 2:'Learn', 3:'Free' ,4:'.co'}
    print(Dict.items())

Output:- 

[(0, 'welcome'), (1, 'to'), (2, 'Learn'), (3, 'Free'), (4, '.co')]





