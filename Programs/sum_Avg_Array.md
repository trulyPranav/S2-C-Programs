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
 ```

 ## Algorithm:

 ### Step 1:Start

 ### Step 2:Initialize a[100],i,sum=0,avg=0,size=0

 ### Step 3:Read Size of Array and store it in size

 ### Step 4:Read the elements of the array by initializing a for loop from i=0 till i<size


### Step 5:Initialize a for loop from i=0 and repeat the below till i<size
#### Step 5.1: sum = sum + a[i]
#### Step 5.2: i++

### Step 6:Display the sum and average
### Step 7:Stop