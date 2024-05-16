## Code:
```c 
#include<stdio.h>
 void main()
 {
  int a[30],i=0,sum=0,avg=0,size=0;
   
  printf("Enter the array size:");
  scanf("%d", &size);                      //determines the size of array
  
  printf("Enter the array elements:");
  for(i=0;i<size;i++)
  {
    scanf("%d",&a[i]);                      
  }

  for(i=0;i<size;i++)
  {
    sum=sum + a[i];                     
  }
  avg=sum/size;                             //if sum=15,limit=5 then avg=(15/5)=3
  printf("Sum of elements: %d", sum);
  printf("\nAverage of elements: %d", avg);
 }