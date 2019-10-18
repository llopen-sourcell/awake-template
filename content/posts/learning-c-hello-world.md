---
title: Learning C | Hello World
subtitle: Learning C | Hello World
category:
  - Programming
author: Daniel Kelly
date: 2019-10-17T15:55:47.772Z
featureImage: /uploads/resource-grid-hero.jpg
---
We come to our very first tutorial on introduction to C.

In this example I will show you how to print to the screen, using our hello world example

```
    #include <stdio.h> 
    int main(){   // This is a comment line
    printf("Hello, World!");
    return 0;
    }
```

Now I don't think there is much need for an explanation of this code

we will include stdio.h so that we can use the function printf for displaying onto the screen.

we use int main() here we can also use void main() but if that is the case no value should be returned at the end of the program

Now let us consider another piece of code where we scan a string and print it

```
   #include<stdio.h>
   void main(){
   char input[10];
   scanf("%s",input);
   printf("%s World!",input);
   }
```

input:- Hello

Output:- Hello World

In the above code we used %s for reading a string, a string reading will be terminated when it reaches a space or null value

similarly %d can be used to input and output integer values

SO what we learned so far in this tutorial is that

printf is a function for printing values on to the scree

```
#include<stdio.h>
void main(){
   int num=10;
   printf("%d",num);// %d is used to print an integer value
}// this code will print 10 as an output
```
