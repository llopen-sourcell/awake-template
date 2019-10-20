---
title: Selection Sort
subtitle: 'Selection Sort in C, Python'
category:
  - Programming
author: Anand Murali
date: 2019-10-20T09:57:29.430Z
featureImage: /uploads/about-hero.jpg
---
Selection Sort

Simple sorting algorithm shich works on <math xmlns="http://www.w3.org/1998/Math/MathML">
  <mi>O</mi>
  <mo stretchy="false">(</mo>
  <msup>
    <mi>N</mi>
    <mn>2</mn>
  </msup>
  <mo stretchy="false">)</mo>
</math> time complexity

Selection sort as its name suggests ,tries to sort an array by selecting the minimum element and placing it at the correct position.

Selection sort will maintain 2 sub arrays one which is sorted and other which is not

Eg:- 
array={10,12,15,9,4,25}

after first iteration the least value 4 will be selected and swapped with first element of array

array={ 4,12,15,10,25 }

Now the sub array {4} is sorted and the other sub array {12,15,10,25} is unsorted

We have to complete these steps until all elements are sorted


Function for selection sort in C
     
    	#include<stdio.h>

	void swap(int *a,int *b)
	{
		int temp=*a;
		*a=*b;
		*b=temp;
	}

	void SimpleSelectionSort(int *a,int length)
	{
		int i,j;
		int min;
		for(i=0;i<length;i++)
		{
			min=i;
			for(j=i+1;j<length;j++)
			{
				if(a[j]<a[min])
				{
					min=j;	
				}
			}
			if(min!=i)
			{
				swap(&a[i],&a[min]);
			}
		
		}
	}




	void arrayTraversal(int *a,int length)
	{
		int i;
		for(i=0;i<length;i++)
		{
			printf("%d ",a[i]);
		}	
		printf("\n");
	}

	void main()
	{
		int a[7]={5,4,3,2,1,7,6};
		SimpleSelectionSort(a,7);
		arrayTraversal(a,7);

		int b[5]={5,3,4,6,2};
		SimpleSelectionSort(b,5);
		arrayTraversal(b,5);
	}

Output: - 
          Sorted array: 
          11 12 22 25 64 

 

Python code for selection sort 

    def select_sort(numbers):
        for i in range(len(numbers)): 
            min_index = i 
            for j in range(i+1, len(numbers)): 
                if numbers[min_index] > numbers[j]: 
                    min_index = j 
           
            numbers[i], numbers[min_index] = numbers[min_index], numbers[i] 
  
    # Driver code to test above 
    if __name__ == "__main__":
        numbers=[10, 12, 25, 224,12,1]
        select_sort(numbers)
        print(numbers)
Output:- 
[1, 10, 12, 12, 25, 224]

