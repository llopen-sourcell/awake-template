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

