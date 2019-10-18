---
title: 'Urlify a given string '
subtitle: replace all spaces with %20
category:
  - Programming
author: Anand Murali
date: 2019-10-17T15:02:08.109Z
featureImage: /uploads/purge-css-hero.jpg
---
Urlify a given string that means replace all spaces with %20. I encountered this problem on a book called Cracking the coding interview and I would like to show two methods of solving this problem.

Input :- "Mr John Smith"

Output:-  "Mr%20John%20Smith"

Method 1

This is the simplest method, all it does is iterate through the string an insert '%20' whenever an space is found.

The code for this method is 

`#python 3`\
`url="   Hello World     "`\
`char=char.strip()`\
`char=char.replace(' ' ,'%20')`\
`print char`

Now there is another case to it

Input :-`"Mr John Smith   ",16`

Output:- `"Mr%20John%20Smith"`

Here we assume there is enough space in the string to accommodate all the extra characters

We use a 2 scan approach to edit the string, In the first pass we only scan the string counting the number of spaces in the string, and by tripling this number we can know how much space is required

ex:-  "hello world" in this string there is only one space and we have to insert 3 characters at that place so we need the length of string to be

length of string + number of spaces *2 

After the first scan we can then scan from the back editing the string as we go

we can see a java implementation of this algorithm below

```
public void replaceSpaces(char[] str, int length) {
```

```
    int spaceCount = 0, newLength, i;
```

```
    for (i = 0; i < length; i++) {
```

```
        if (str[i] == ' ') {
```

```
            spaceCount++;
```

```
        }
```

```
    }
```

```
    newLength = length + spaceCount * 2;
```

```
    str[newLength] = '\0';
```

```
    for (i = length - 1; i >= 0; i--) {
```

```
        if (str[i] == ' ') {
```

```
            str[newLength - 1] = '0';
```

```
            strfnewLength - 2] = '2';
```

```
        str[newLength - 3] = '%';
```

```
        newLength = newLength - 3;
```

```
    } else {
```

```
        str[newLength - 1] = str[i];
```

```
        newLength = newLength - 1;
```

```
    }
```

```
}
```

```
}
```
