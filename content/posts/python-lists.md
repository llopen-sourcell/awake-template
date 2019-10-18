---
title: 'Python - Lists '
subtitle: Data Structures in python
category:
  - Programming
author: Anand Murali
date: 2019-10-18T17:03:31.393Z
featureImage: /uploads/contact-hero.jpg
---
Python Lists

List is a data structure in python which can be used to store any tpe of data.A same list can have diffrent data types
List is declared as
list_name=[]

     list1=[1,'Hello',21.09]

Inserting

To insert elements to a list we can use the built in insert()

Syntax :- list_name(index,value)

     list1=[1,'Hello',120]
     list1.insert(1,'hai')
     print list1

Output :- [1, 'hai', 'Hello', 120]

Here when we insert into index 1, the value is added to that index without any value being overwritten

Deleting

Syntax :- del list_name[index]

    list1=[1, 'hai', 120]
    del list1[2]
    print list1

Output:-[1, 'hai']


Appending

list_name.append(value)
Updating
Merging two lists
Printing a List
Basic Operations
Built in List functions


 	cmp(list1, list2)

Compares elements of both lists.
2 	len(list)

Gives the total length of the list.
3 	max(list)

Returns item from the list with max value.
4 	min(list)

Returns item from the list with min value.
5 	list(seq)

Converts a tuple into list.

Python includes following list methods
Sr.No. 	Methods with Description
1 	list.append(obj)

Appends object obj to list
2 	list.count(obj)

Returns count of how many times obj occurs in list
3 	list.extend(seq)

Appends the contents of seq to list
4 	list.index(obj)

Returns the lowest index in list that obj appears
5 	list.insert(index, obj)

Inserts object obj into list at offset index
6 	list.pop(obj=list[-1])

Removes and returns last object or obj from list
7 	list.remove(obj)

Removes object obj from list
8 	list.reverse()

Reverses objects of list in place
9 	list.sort([func])

Sorts objects of list, use compare func if given
