## Code:
```c
#include <stdio.h>

void main(){
    int i,n,sum=0,avrg=0,a[100];
    printf("Enter the number of elements in the array:");
    scanf("%d",&n);
    printf("Enter the elements of the array:");
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    // Adding the elements
    for(i=0;i<n;i++){
        sum+=a[i]; // sum = sum + a[i];
    }
    avrg = sum/n;
    printf("%d is the sum of the array\n", sum);
    printf("%d is the average of the array", avrg);
}
```
## Algorithm:

### Step 1: Start

### Step 2: Initialize i,n,avrg=0,sum=0 and a[100]

### Step 3: Read the array size and store it in n

### Step 4: Read the array elements by initializing a for loop from i=0 till i<n

### Step 5: Initialize a for loop from i=0 till i<n

#### Step 5.1: sum = sum + a[i]

#### Step 5.2: increment i by 1

### Step 6: avrg = sum/n

### Step 7: Display sum and avrg

### Step 8: Stop