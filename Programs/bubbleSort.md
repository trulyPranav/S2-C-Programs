## Code:
```c
#include <stdio.h>

void main(){
    // Initializing and reading the Array
    int i=0,j=0,temp=0,lim,a[100];
    printf("Enter the size of the array:");
    scanf("%d", &lim);
    printf("Enter the elements of the array:");
    for(i=0;i<lim;i++){
        scanf("%d", &a[i]);
    }
    // Bubble Sorting:
    for(i=0;i<lim-1;i++){
        for(j=0;j<lim-1-i;j++){
            // Swapping if a[j]>a[j+1]
            if(a[j]>a[j+1]){
                temp=a[j];
                a[j]=a[j+1];
                a[j+1]=temp;
            }
        }
    }
    printf("Sorted Array:")
    for(i=0;i<lim;i++)
    {
        printf("%d ", a[i]);
    }
}

```

## Algorithm:

### Step 1: Start

### Step 2: Initialize a[100],i,j,lim,temp

### Step 3: Read the size of array and store it in lim

### Step 4: Input array elements using a for loop

### Step 5: Initialize a for loop from i=0 till i<lim-1

#### Step 5.1: Initialize a for loop from j=0 till j < lim-i-1 and do the following if a[j]>a[j+1]
<pre>
Step 5.1.1:
    temp = a[j];
    a[j] = a[j+1];
    a[j+1] = temp;
</pre>

### Step 6: Display the Sorted Array

### Step 7: Stop

